# sorting
Selection sort in cpp
#include <iostream>
using namespace std;
void display(int array[],int size)
{
	int i;
	for(i=0;i<size;i++)
	{
		cout<<array[i]<<"\t";
 
	}
	cout<<'\n';
}
 
int main() {
	int array[]={5,3,1,9,8,2,4,7};
	int size=sizeof(array)/sizeof(array[0]);
	cout<<"Before swapping array is:::"<<endl;
	display(array,size);
	int i,j,min,temp;
	for(i=0;i<size-1;i++)
	{
		min=i;
		for(i=0;i<size-1;i++)
		{
			if(array[j]<array[min])
			min=j;
		}
		temp=array[min];
		array[min]=array[i];
		array[i]=temp;
 
	}
	cout<<"After swapping array is"<<endl;
	for(i=0;i<size;i++)
	{
	display(array,size);
	}
	// your code goes here
	return 0;
  }
