# Bài tập chương 3
#### Bài 2: Viết chương trình nhập vào số nguyên dương **n** (n <= 100). Tính và hiển thị tổng các số tự nhiên lẻ từ 1 đến n.

Ví dụ:
```
n = 10
Ket qua la 25
```

```c++
#include <iostream>
using namespace std;
int main()
{
	int n;
	cout << "n = ";
	cin >> n;
	
	int s = 0;
	
	for (int i = 1; i <= n; i += 2)
	{
		s = s + i;
	}
	cout << "Ket qua la " << s;
	
	return 0;
	
}

```
---
#### Bài 3: Viết chương trình nhập nhiệt độ F từ bàn phím rồi tính và hiển thị nhiệt độ đó ở độ C

Gợi ý:
- degC = (degF - 32) / 1.8

Ví dụ:
```
F = 80 
C = 26.6667
```

```c++
#include <iostream>
using namespace std;
int main()
{
	//degC = (degF - 32) / 1.8
	
	float C, F;
	cout << "F = ";
	cin >> F;
	
	C = (F - 32) / 1.8;
	
	cout << "C = " << C;

	return 0;
	
}
```

---

#### Bài 4: Viết chương trình nhập vào một số **n** từ bàn phím. Hãy kiểm tra xem **n** có phải số nguyên tố hay không.

Gợi ý:
- Số nguyên tố là số chỉ chia hết cho 1 và chính nó.

Ví dụ:
```
n = 3
n la so nguyen to
```

```c++
#include <iostream>
using namespace std;
int main()
{
	int n;

	cout << "n = ";
	cin >> n;
	
	bool is_nt = true;
	
	for (int i = 2; i < n - 1; i++)
	{
		if (n % i == 0)
		{
			is_nt = false;
			break;
		}
	}
	
	if (is_nt)
	{
		cout << "n la so nguyen to";
	}
	else {
		cout << "n khong la so nguyen to";
	}
	return 0;
	
}
```
---

#### Bài 5: Viết chương trình nhập vào một số nguyên dương n từ bàn phím. Tính tổng các chữ số tạo nên số đó.

Ví dụ:
```
n = 2023
Ket qua la 7
```

```c++
#include <iostream>
using namespace std;
int main()
{
	int n;
	cout << "n = ";
	cin >> n;
	
	// 2023 % 10 = 3
	// 2023 / 10 = 202
	// 202 % 10 = 2
	// 202 / 10 = 20
	// 20 % 10 = 0
	// 20 / 10 = 2
	// 2 % 10 = 2
	
	int sum = 0;
	while(n > 0)
	{
		sum += (n % 10); // Tach so ra
		n /= 10; // Thanh so da tach
	}
	cout << "Ket qua la " << sum;
	
	return 0;
	
}
```
