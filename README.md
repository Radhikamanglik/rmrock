#include<stdio.h>
#include<conio.h>
#include<dos.h>
#include<stdlib.h>
void main()
{
    int choice1,choice2,rock,paper,scissor;
    char ch;
    do
    {
        clrscr();
        printf("1.rock\n2.paper\n3.scissor");
        printf("enter user choice=");
        scanf("%d",&choice1);
        choice2=rand()%3;
        delay(200);
        printf("computer choice=%d\n",choice2);
        if(choice1==1)
        {
            if(choice2==1)
           { printf("draw\n");}   
           if(choice2==2)
           { printf("computer wins\n");}
           if(choice2==3)
           { printf("user wins\n");}
        }
        else if(choice1==2)
        {
            if(choice2==2)
            { printf("draw\n");}
            if(choice2==3)
            { printf("computer wins\n");}
            if(choice2==1)
            { printf("user wins\n"); }
        }
        else if(choice1==3)
        {
            if(choice2==3)
            { printf("draw\n"); }
            if(choice2==1)
            { printf("computer wins\n"); }
            if(choice2==2)
            { printf("user wins\n"); }
        } 
        else
            { printf("invalid choice"); }
        delay(500);
        printf("do you want to continue y/n=");
        ch=getche();
    }
  while(ch=='Y' || ch=='y');
  getch();
 } 
  
        
