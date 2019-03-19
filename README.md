#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int n;
    scanf("%d",&n);
    if(n>=1 && n<=8){
    for(int i=1;i<=n;i++)
    {
        for(int j=1;j<=2*n+1;j++)
        {
            if(j==n+1 || j<=n-i || j>=n+i+2)
                printf(" ");
            else
                printf("#");
        }
        printf("\n");
    }}
    else
        return 0;
}
