//selection sort//
#include<iostream>

using namespace std;

int main()
{
    int n=10,arr[n];

    int min_index,temp;

    
    cout<<"enter element";
    for(int i=0;i<n;i++){
        cin>>arr[i];

    }

    for (int i = 0; i < (n-1); i++)
    {
        min_index=i;
        for (int j = i+1; j < n; j++)
        {
            if(arr[min_index]>arr[j])
            min_index=j;

        }
        

    

    if(min_index!=i) {
    temp=arr[i];
    arr[i]=arr[min_index];
    arr[min_index]=temp;


    }

    }


for (int i = 0; i < n; i++)
{
    cout<<"  "<<arr[i];

}
return 0;

}
