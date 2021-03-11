
#include<stdio.h>
int main()
{
    int i ,j, k,n;
    int arr1[100];
    printf("Input the size of array:");
    scanf("%d",&n);
    for(i = 0; i<n; i++)
    {
        printf("Elements %d = ",i);
        scanf("%d",&arr1[i]);
    }
    for(i=0; i<n; i++)
    {
        for(j=0; j<n-1; j++)
        {
            if(arr1[j] <arr1[i])
            {
                k = arr1[i];
                arr1[i] = arr1[j];
                arr1[j] = k;
            }
        }
   }
    for(i = 0;  i<n; i++)
      {
          printf("%d",arr1[i]);
      }
      return 0;
}
