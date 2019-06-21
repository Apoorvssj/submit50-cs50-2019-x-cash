# submit50-cs50-2019-x-cash 
#include<cs50.h>
#include<stdio.h>
#include<math.h>
int main(void)
{
    float dollars;float cents; int counter=0;int n=0;
    
    do{
        dollars=get_float("change owed:");
       
       
    }while(dollars<0);
     cents=round(dollars*100); 
    n=cents;
    
    
    while(n>=25)
    {
        n=n-25;
        counter++;
    }
    while(n>=10)
    {
        n=n-10;
        counter++;
    }
    while(n>=5)
    {
        n=n-5;
        counter++;
    } 
    while(n>=1)
    {
        n=n-1;
        counter++;
    } 
    
    printf("coins given:%i\n",counter);
    
}
