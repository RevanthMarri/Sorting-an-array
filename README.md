#include<stdio.h>
int main()
{
    int arr[20],size,i,j,temp;
    printf("enter the size of array=");
    scanf("%d",&size);
    printf("enter the elements of array");
    for(i=0;i<size;i++)
    {
        printf("\n enter the %d elements:",i+1);
        scanf("%d",&arr[i]);
    }
    printf("\n Sorted array is:");
    for(i=0;i<size;i++)
    {
        for(j=0;j<size;j++)
        {
            if(arr[i]>arr[j+1])
            {
                temp=arr[i];
                arr[i]=arr[j+1];
                arr[j+1]=temp;
            }
        }   
    }
    printf("\n enterd array is:");
    for(i=0;i<size;i++)
    printf("\t%d",arr[i]);
    printf("\n array is %d iteration:",j+1);
    for(j=0;j<size;j++)
    printf("\t%d",arr[j]);
return 0;
}
