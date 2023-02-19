# cpp_tutorial
### Nhập vào 2 số nguyên dương `a` và `b` (a và b không trùng giá trị). Hãy in ra màn hình số nhỏ hơn (dùng toán tử 3 ngôi)
   
   	#include <iostream>

    	using namespace std;
    	int main()
    	{

	int a, b, c;
   	 cout << "a = ";
	cin >> a;
	cout << "b = ";
	cin >> b;
	
        c = (a < b) ? a : b; 
	
    	/* Ði tu` dâ'u ? ra: a < b không?
	//Ðúng thì là c = a
	//Sai thì là c = b
	*/	
	
   	 cout << "Gia tri nho hon la " << c;
	
   	 return 0;
   	 }
