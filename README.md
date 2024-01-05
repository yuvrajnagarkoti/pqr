BASIC C PROGRAMMING RECURSIVE CODE FOR FIBONACCI SERIES TILL LIMIT N



#include <stdio.h>
int fibbo(int);
void main()
{
    int sum=0,n,k,i;
    printf("enter limit");
    scanf("%d",&n);
    for( i=0 ; i<=n ; i++ )
    {
        k=fibbo(i);
        printf("%d",k);
    }
}

int fibbo(int n)
{
    if(n<=1)
    {
        return n;
    }
    else
    {
        return fibbo(n-1)+fibbo(n-2);
    }
}
