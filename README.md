# RA2111009010195
ATM system

******

#include <stdio.h>

int main() {

    int pin,choice,withdraw,balance,fastcash;
    
    printf("Welcome To XYZ Bank");
    printf("\nPlease Enter 4-digit PIN Number");
    scanf("%d", &pin);
    
    if (pin==1234){
        printf("\nPlease Choose Service");
        printf("\n1- Withdrawal");
        printf("\n2- Check Balance");
        printf("\n3- Fast Cash");
    }
    else printf("\nIncorrect PIN\nPlease Enter Correct PIN.");
    
    scanf("%d", &choice);
    scanf("%d", &balance);
    
    if(choice==1){
        printf("\nPlease Enter Withdrawal Amount");
        printf("\nEnter Amount in Multiples of 100");
        scanf("%d", &withdraw);
        if(withdraw<balance&& withdraw%500==0){
            printf("\nPlease Collect Cash");
        }
        else printf("\nInvalid Amount\nEnter Valid Amount");}
        
    if(choice==2){
        printf("\nAvailable Bank Balance= Rs. %d", balance);
    }
    
    if(choice==3){
        printf("\n Please Choose Fast Cash Option:");
        printf("\n1- Rs.5000");
        printf("\n2- Rs.10000");
        printf("\n3- Rs.15000");
        printf("\n4- Rs.20000");}
        
       scanf("%d", &fastcash);
        
        if(fastcash==1){
            if(5000<=balance){printf("\nPlease Collect Cash");
        }
        else printf("\nInsufficient Balance");}

        if(fastcash==2){
           if(10000<=balance){ printf("\nPlease Collect Cash");
        }
        else printf("\nInsufficient Balance");}

        if(fastcash==3){
            if(15000<=balance){printf("\nPlease Collect Cash");
        }
        else printf("\nInsufficient Balance");}

        if(fastcash==4){
            if(20000<=balance){printf("\nPlease Collect Cash");
        }
        else printf("\nInsufficient Balance");}

    
if(choice>3){printf("\nInvalid Service.");}
    
    return 0;}

