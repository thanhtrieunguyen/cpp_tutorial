# cpp_tutorial
## In ra số `lẻ` từ `1` đến `9`
                #include <iostream>
                using namespace std;
                int main() {

                #if 0

                //	for ( int i = 1; i <= 9; i += 2)
                //	{
                //		cout << i << endl;
                //	}
                #endif

                #if 0
                        int i = 1;
                        while (i <= 9 ) {
                                cout << i << endl;
                                i += 2;
                        }
                #endif

                #if 1 
                        int i = 1;
                        do 
                        {
                                cout << i << endl;
                                i += 2;
                        }
                        while (i <= 9);
                #endif

                        system("pause");
                        return 0;
                }
