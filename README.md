# problems-on-array#include<iostream>
using namespace std;


bool fun(int ar[] , int size){

     for(int st = 0; st < size;st++){

    for(int end = (st+1);end< size;end++){

        if(ar[st] == ar[end]){
            return true;
        }

    }
}
return false;
}

int main(){

    int n;

    cout<<"enter number =";
    cin>>n;

   int arr[n];

   int len = sizeof(arr)/sizeof(arr[0]);

   for(int i=0; i<n;i++){
    cin>>arr[i];
   }
   
 bool result =   fun(arr , len);


 cout<<boolalpha; //Use boolalpha to print true/false clearly.

 cout<<result;


    return 0;
}
