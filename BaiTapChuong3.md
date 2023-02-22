# Bài tập chương 3
<p> Bài 2: Viết chương trình nhập vào số nguyên dương <b> n </b> (n <= 100). Tính và hiển thị tổng các số tự nhiên lẻ từ 1 đến n </p>

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
