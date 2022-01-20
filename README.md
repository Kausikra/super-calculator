#include<stdio.h>
int main()
{
    int choice,a,b;
    printf("\t welcome to super calculator by srm university");
    printf("\n please enter 1 to add two numbers");
    printf("\n please enter 2 to subract two numbers");
    printf("\n please enter 3 to multiply two numbers");
    printf("\n please enter 4 to division two numbers");
    printf("\n please enter 5 to get the average of the numbers:");
    printf("\n please enter 6 to print the numbers between the given values:");
    printf("\n please enter 7 to find whether the number is positive or not:");
    printf("\n enter the value for a:");
    scanf("%d",&a);
    printf("enter the value for b:");
    scanf("%d",&b);
    printf("\n enter the choice that what operation it has to do:");
    scanf("%d",&choice);
    switch(choice)
    {
        case 1:
        printf("\n the addition for the given number is %d",a+b);
        break;
        case 2:
        printf("\n the subraction for the given number is %d",a-b);
        break;
        case 3:
        printf("\n the multiplication of the given number is %d",a*b);
        break;
        case 4:
        printf("\n the division of the given number is %d",a/b);
        break;
        case 5:
        printf("\n the average of the given number is %d",a+b/2);
        break;
        case 6:
        {    
            for(a;a<=b;a++)
            {
            printf("\n the loop  is %d",a);
            }
        }    
        break;
        case 7:
        {
            if(a>0 && b>0)
            printf("\n both the numbers are positive %d %d",a,b);
            else if(a>0 && b<0)
            printf("\n a is positive and b is negative");
            else if(a<0 && b>0)
            printf("\n a is negative and b is positive");
            else
            printf("\n both the numbers you have given is negative");
        }
        break;
        default:
        printf("\n sorry you have entered an invalid choice:");
        break;
        return 0;
    }
}
