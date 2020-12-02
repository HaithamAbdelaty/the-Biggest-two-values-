# the-Biggest-two-values-
as you have an array , find the maximum value of the array and the second maximum value 
#include <iostream>
using namespace std;
int main ()
{
const int size=6; int arr[size]={4,5,2,3,1};
int max1,max2; 
if(arr[0]>=arr[1])
    max1=arr[0],max2=arr[1];
else
    max1=arr[1],max2=arr[0];
for(int i=2;i<size;i++)
{
    if(max1<=arr[i])
        max2=max1 , max1=arr[i];
    else if (max2<arr[i])
        max2=arr[i];


}
cout<<max1<< "  "<< max2<<endl;
}
