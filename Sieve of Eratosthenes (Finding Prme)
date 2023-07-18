#include<iostream>
#include<vector>
using namespace std;

void printArr(vector<bool> arr, int n){
    for(int i=0; i<n; i++){
        cout << arr[i] << ' ';
    }
    cout << endl;
    for(int i=0; i<n; i++){
        cout << i << ' ';
    }
    cout << endl;
}

int main(){
    int n;
    cout << "Enter a number" << endl;
    cin >> n;
    
    vector<bool> is_prime(n+1, true);
    is_prime[0] = is_prime[1] = false;
    for (int i = 2; i <= n; i++) {
        if (is_prime[i] && (long long)i * i <= n) {
            for (int j = i * i; j <= n; j += i)
                is_prime[j] = false;
        }
    }
    printArr(is_prime, n);
    
    return 0;
}
