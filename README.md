/*#lockercalculation
This program just collect $10,$50 and $100 only.Then it will finally gives the total amount in locker.*/
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int n,i,total;
    int pathunote=0;
    int ambathunote=0;
    int noorunote=0;
    for(i=0;i<=2;i++)
    {
    scanf("%d",&n);
    if((n==10)||(n==50)||(n==100))
        {
        if(n==10)
        {
            pathunote=pathunote+1;
        }
        else if(n==50)
        {
            ambathunote=ambathunote+1;
        }
        else if(n==100)
        {
            noorunote=noorunote+1;
        }
    }
    }
    printf("Total 10 Rupees note is %d \n",pathunote);
    printf("Total 50 Rupees note is %d \n",ambathunote);
    printf("Total 100 Rupees note is %d \n",noorunote);
    total=((pathunote*10)+(ambathunote*50)+(noorunote*100));
    printf("Total 10 Rupees note is %d \n",total);
    return 0;
}
