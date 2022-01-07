#include <stdio.h>

int main() {
int b;
float HL,CL,BL,SL,LP,a,res;
do{
printf("*Welcome to Loan Management System*\n\n");
printf("   MAIN MENU\n");
printf("================\n");
printf("LOAN CALCULATOR:-\n\n");
printf("[1] HOME LOAN\n");
printf("[2] CAR LOAN\n");
printf("[3] BUSINESS LOAN\n");
printf("[4] STUDENT LOAN\n");
printf("[5] LOAN AGAINST PROPERTY\n");
printf("Enter your choice:");
scanf("%d",&b);
 switch(b){
    case 1:
    printf("enter the loan amount:\n");
    scanf("%f",&a);
    HL=a+2.6*a;
    res=HL;
    break;
    case 2:
    printf("enter the loan amount:\n");
    scanf("%f",&a);
    CL=a+3.2*a;
    res=CL;
    break;
    case 3:
    printf("enter the loan amount:\n");
    scanf("%f",&a);
    BL=a+4.2*a;
    res=BL;
    break;
    case 4:
    printf("enter the loan amount:\n");
    scanf("%f",&a);
    SL=a+1.9*a;
    res=SL;
    break;
    case 5:
    printf("enter the loan amount:\n");
    scanf("%f",&a);
    LP=a+2.5*a;
    res=LP;
    break;
    default:
    printf("invalid input\n");
    printf("try again\n\n");
    break;
}
}while(b<1 || b>5);
 printf("Your amount to be submitted at the required rate of interest is:\nRs. %.4f\n\n",res);
 int m;
    printf("  EMI PAYMENT\n");
    printf("===============\n");
    printf("EMI CALCULATOR:-\n\n");
    printf("[1] 6 monthly installment\n");
    printf("[2] 8 monthly installment\n");
    printf("[3] 12 monthly installment\n");
    printf("[4] Exit\n");
    printf("Choose your mode of payment:\n");
    scanf("%d",&m);
    float hlf,quat,yrly,j;
    hlf = res / 6;
    quat = res /8;
    yrly = res/12;
    if (m == 1){
       j = hlf;
    printf("your return payement for the required loan amount is:\nRs.%.4f for 6 monthly installments\n\n",j);
    }
    else if (m == 2){
       j = quat;
    printf("your return payement for the required loan amount is:\nRs.%.4f for 8 monthly installments\n\n",j);
    }
    else if (m == 3){
       j = yrly;
    printf("your return payment for the required loan amount is:\nRs.%.4f for 12 monthly installments\n\n",j);
    }
    else
       printf("RETURN TO THE MAIN MENU\n\n");
    printf("****Thank you for choosing XYZ bank😊****");
    return 0;
}
