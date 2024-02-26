//new-del-fnc
#include <iostream>
using namespace std;

int main() {
    int *pInt = new int;
    int x;
    cin>>x;
    *pInt = x;
    cout << "Value of *pInt: " << *pInt << endl;
    delete pInt;
    int *pIntArray = new int[5];
    for (int i = 0; i < 5; i++) {
        pIntArray[i] = i * 10;
    }
    for (int i = 0; i < 5; i++) {
        cout << "Value of pIntArray[" << i << "]: " << pIntArray[i] << endl;
    }
    delete[] pIntArray;
    return 0;
}
