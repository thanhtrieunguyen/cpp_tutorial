# cpp_tutorial
#### Bài 1: Tạo mảng số nguyên dương có n phần tử (tối đa 10 phần tử). Nhập vào 1 số nguyên dương x và thêm x vào cuối mảng vừa tạo.
````c++
#include <iostream>
using namespace std;

int main()
{
	int n, x;
	cout << "n = ";
	cin >> n;
	cout << "x = ";
	cin >> x;
	int numbers[n];
	
	for (int i = 0; i < n; i++)
	{
		cout << "Numbers [" << i << "] = ";
		cin >> numbers[i]; 
	}
	cout << endl;
		for (int i = 0; i < n; i++)
	{
		cout << "Numbers [" << i << "] = " << numbers[i] << x << endl;
	}
	
	return 0;
}
````
