# 100-days-challenge
100 days C programming challenge

Q1: Write a program to input two numbers and display their sum.

#include <stdio.h>
int main()
{
    int num1,num2,sum;
    printf("ENTER THE FIRST NUMBER: ");
    scanf("%d" , &num1);
    printf("ENTER THE SECOND NUMBER: ");
    scanf("%d" , &num2);
    sum= num1+num2;
    printf("THE SUM OF %d and %d is %d/n", num1,num2,sum);
    return0;
}
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/31fe7d9c-45fc-4b6b-b92a-c0fa9e827560" />


Q2: Write a program to input two numbers and display their sum, difference, product, and quotient.

#include <stdio.h>
int main()
{
    float num1,num2,sum,diff,product,quotient;
    printf("ENTER THE FIRST NUMBER: ");
    scanf("%f" , &num1);
    printf("ENTER THE SECOND NUMBER: ");
    scanf("%f" , &num2);
    sum= num1+num2;
    diff= num1-num2;
    product= num1*num2;
    quotient=num1/num2;
    printf("SUM=%f DIFFERENCE=%f PRODUCT=%f QUOTIENT=%f/n", sum,diff,product,quotient);
    return0;
}
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/01530501-6059-414e-8e46-56ac4d152b6b" />



Q3: Write a program to calculate the area and perimeter of a rectangle given its length and breadth.

#include <stdio.h>
int main()
{
    float L,B,A,P;
    printf("ENTER THE LENGTH OF RECTANGLE: ");
    scanf("%f" , &L);
    printf("ENTER THE BREADTH OF RECTANGLE: ");
    scanf("%f" , &B);
    A= L*B;
    P= 2*(L+B);
    printf("AREA=%f PERIMETER=%f/n", A,P);
    return0;
}

Q4: Write a program to calculate the area and circumference of a circle given its radius.

#include <stdio.h>
int main()
{
    float R,A,C;
    float P=3.14;
    printf("ENTER THE RADIUS OF CIRCLE: ");
    scanf("%f" , &R);
    A= P*R*R;
    C= 2*P*R;
    printf("AREA=%f CIRCUMFERENCE=%f/n", A,C);
    return0;
}

Q5: Write a program to convert temperature from Celsius to Fahrenheit.

#include <stdio.h>
int main()
{
    float C,F;
    printf("ENTER THE TEMPREATURE IN DEGREE CELSIUS: ");
    scanf("%f" , &C);
    F=(9/5 * C)+32;
    printf("TEMPERATURE IN DEGREE FAHRENHEIT =%f/n", F);
    return0;
}


Q6: Write a program to swap two numbers using a third variable.

#include <stdio.h>
int main()
{
    int a,b,c;
    printf("ENTER THE FIRST NUMBER: ");
    scanf("%d" , &a);
    printf("ENTER THE SECOND NUMBER: ");
    scanf("%d" , &b);
    c=a;
    a=b;
    b=c;
    printf("NUMBERS AFTER SWAPPING= %d  %d/n", a,b);
    return0;
}

Q7: Write a program to swap two numbers without using a third variable.

#include <stdio.h>
int main()
{
    int a,b;
    printf("ENTER THE FIRST NUMBER: ");
    scanf("%d" , &a);
    printf("ENTER THE SECOND NUMBER: ");
    scanf("%d" , &b);
    a=a+b;
    b=a-b;
    a=a-b;
    printf("NUMBERS AFTER SWAPPING= %d  %d/n", a,b);
    return0;
}

Q8: Write a program to find and display the sum of the first n natural numbers.

#include <stdio.h>
int main()
{
    int n,sum;
    printf("ENTER THE VALUE OF n: ");
    scanf("%d" , &n);
    sum= n*(n+1)/2;
    printf("SUM OF FIRST %d NATURAL NUMBERS = %d/n", n,sum);
    return0;
}

Q9: Write a program to calculate simple and compound interest for given principal, rate, and time.

#include <stdio.h>
int main()
{
    float p,r,t,S.I,C.I,A;
    printf("ENTER PRINCIPAL: ");
    scanf("%f" , &p);
    printf("ENTER TIME: ");
    scanf("%f" , &t);
    printf("ENTER RATE: ");
    scanf("%f" , &r);
    S.I= p*r*t/100;
    A= p*pow((1+r/100),t);
    C.I= A-p;
    printf("SIMPLE INTEREST= %f  COMPOUND INTEREST= %f/n", S.I,C.I);
    return0;
}


Q10: Write a program to input time in seconds and convert it to hours:minutes:seconds format.

#include <stdio.h>
int main()
{
    int time,hrs,mins,secs;
    printf("ENTER TIME IN SECONDS: ");
    scanf("%d" , &time);
    hrs= time/3600;
    mins= (time%3600)/60;
    secs= time%60;

    printf("TIME= %d:%d:%d/n", hrs,mins,secs);
    return0;
}   

Q11: Write a program to input an integer and check whether it is even or odd using if–else.

  #include <stdio.h>
  int main()
  {
     int a ;
     printf("ENTER AN INTEGER VALUE: ");
     scanf("%d" , a);
     if (a%2 == 0)
     {
       printf("THE NUMBER ENTERED IS EVEN.");
    }
    else
    {
      printf("THE NUMBER ENTERED IS ODD.");
    }
    return 0;
}
     
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/941ba982-7c21-43b2-b6ba-4928240a030b" />

Q12: Write a program to input an integer and check whether it is positive, negative or zero using nested if–else.

  #include <stdio.h>
  int main()
  {
     int a  ;
     printf("ENTER AN INTEGER VALUE: ");
     scanf("%d" , &a);
     
    
     if (a >= 0)
     {
        if(a==0)
        {
            printf("THE NUMBER ENTERED IS ZERO.");
        }
        else
        {
            printf("THE NUMBER ENTERED IS POSITIVE.");
        }
    }
    else
    {
      printf("THE NUMBER ENTERED IS NEGATIVE.");
    }
    return 0;
}
     
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/b93c977c-8b12-4858-ace7-fd4b47c641a5" />

