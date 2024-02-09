# hash_map

// Online C++ compiler to run C++ program online
#include <iostream>
#include <unordered_map>
#include <map>
using namespace std;
int main() {
    int n=10;
    map<int, int>mpp;
    int arr[n]={2,7,5,12,9,2,4,7,5, 5, 5};
    for(int i=0;i<n;i++){
        mpp[arr[i]]++;
    }
    //iteration of map
    for(auto it:mpp){
        cout<<it.first<<"->"<<it.second<<endl;
    }
    int q;
    cin>>q;
    int num;
    while(q--){
        cin>>num;
        cout<<mpp[num]<<endl;
    }
    return 0;
}
