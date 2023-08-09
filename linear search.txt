#include<stdio.h>
int main()
{
	int n,arr[100],ele,i;
	printf("Enter the no of elements:");
	scanf("%d",&n);
	printf("Enter the elements:");
	for(i=0;i<n;i++)
	{
		scanf("%d",&arr[i]);
	}
	printf("Enter the element to search:");
	scanf("%d",&ele);
	for(i=0;i<ele;i++)
	{
		if (arr[i]==ele)
		{
			printf(" %d is found at the position %d",ele,i);
			break;
		}
		
	}
	if(i==ele)
		printf("NOT Found");
	
	return 0;
}
