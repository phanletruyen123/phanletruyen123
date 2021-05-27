#include<stdio.h>
#include<stdlib.h>

int main()
{
    int m,n,i,j,bien;
    scanf("%d %d",&m,&n);
    int x[100][100];
    int (*p)[100];
    p=x;
    for(i=0;i<m;i++)
    {
       for(j=0;j<n;j++)
       {
           scanf("%d",&bien);

           *(*(p+i)+j) = bien;

       }
    }
    for(i=0;i<m;i++)
    {
        for(j=0;j<n;j++)
        {
            printf("%5d",x[i][j]);
        }
        printf("\n");
    }
}

/// Hai chieu


#include <stdio.h>
#include <math.h>
int main()
{
    int i,n, a[100];
    scanf("%d",&n);
    for (i=0; i<n; i++)
    {
        int tg;
        printf ("\n Phan tu %d, I+1");
        scanf("%d",&tg);
        *(a+i) = tg;  // gia tri tg gán vào pha  tư trong mang a
    }
    for(i=0;i<n;i++)
        {
            printf("%d",a[i]);
        }
}
/// Mot chieu
