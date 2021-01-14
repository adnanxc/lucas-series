# lucas-series

#include <iostream>
using namespace std;


int main(){
    int n;
    cout << "Enter the number of terms N: ";
    cin >> n;
    int t1 = 2, t2 = 1 , t3 = 0;

    if(n==1){
        cout << t1;
    }

    if(n==2){
        cout << t1 << " , " << t2 << " , ";
    }

    else{
        cout << t1 << " , " << t2;
        for(int i=0; i<n-2; i++){
                t3 = t2 + t1;
                t1 = t2;
                t2 = t3;


            cout << " , "<< t3;

        }

    }

}
