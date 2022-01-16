#include<stdio.h>
int main()
{
    printf("Enter a Number \n");
    scanf("%d",&n);
    temp=n;
    while(temp>0)
    {
        sum+=temp%10;
        temp=temp/10;
    }
    temp=sum;
    while(temp>0)
    {
        rev=rev*10+temp%10;
        temp=temp/10;
    }
     if(rev*sum == n)
        printf("Magic Number \n");
    else
        printf("Not a Magic Number \n");
    return 0;
}
