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

Q13: Write a program to input a year and check whether it is a leap year or not using conditional statements.

#include <stdio.h>

int main() 
{
    int year;
    printf("Enter a year: ");
    scanf("%d", &year);
    if ((year % 400 == 0) || ((year % 4 == 0) && (year % 100 != 0)))
    {
        printf("Leap year\n");
    } 
    else 
    {
        printf("Not a leap year\n");
    }

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/78cf5691-78d6-4e3a-b9f0-dc39510d3e4d" />

Q14: Write a program to input a character and check whether it is a vowel or consonant using if–else.

#include <stdio.h>

int main()
 {
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);

    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
        ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U')
    {
        printf("Vowel\n");
    } 
    else
    {
        printf("Consonant\n");
    }

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/e188b02e-36b5-4c01-8e97-af10cb5c07a1" />

Q15: Write a program to input a character and check whether it is an uppercase alphabet, lowercase alphabet, digit, or special character.

#include <stdio.h>

int main() 
{
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);

    if (ch >= 'A' && ch <= 'Z')
    {
        printf("Uppercase alphabet\n");
    } 
    else if (ch >= 'a' && ch <= 'z') 
    {
        printf("Lowercase alphabet\n");
    } 
    else if (ch >= '0' && ch <= '9')
    {
        printf("Digit\n");
    } 
    else 
    {
        printf("Special character\n");
    }

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/540dc0ba-e9ec-42b5-9823-45387bbeca87" />

Q16: Write a program to input three numbers and find the largest among them using if–else.

#include <stdio.h>

int main() 
{
    int a, b, c;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &a, &b, &c);

    if (a >= b && a >= c) 
    {
        printf("Largest is %d\n", a);
    }
    else if (b >= a && b >= c)
    {
        printf("Largest is %d\n", b);
    }
    else 
    {
        printf("Largest is %d\n", c);
    }

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/88c63db3-6969-4a46-b335-f3902b8904c5" />

Q17: Write a program to find the roots of a quadratic equation and categorize them.

#include <stdio.h>
#include <math.h>
int main()
 {
    float a, b, c, D, root1, root2, realPart, imagPart;
    printf("Enter coefficients a, b and c: ");
    scanf("%f %f %f", &a, &b, &c);
     
    D = (b * b) - (4 * a * c);
     if (D > 0)
    {
        root1 = (-b + sqrt(D)) / (2 * a);
        root2 = (-b - sqrt(D)) / (2 * a);
        printf("Roots are real and different: %.2f, %.2f\n", root1, root2);
    }
    else if (D == 0)
    {
        root1 = -b / (2 * a);
        printf("Roots are real and same: %.2f\n", root1);
    }
    else 
    {
        realPart = -b / (2 * a);
        imagPart = sqrt(-D) / (2 * a);
        printf("Roots are complex: %.2f + %.2fi , %.2f - %.2fi\n", realPart, imagPart, realPart, imagPart);
    }
     return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/6a2e4396-719c-42f8-b782-fb2abd294496" />

Q18: Write a program that accepts a percentage (0-100) and assigns a grade based on the following criteria: 
90-100: Grade A 
80-89: Grade B 
70-79: Grade C 
60-69: Grade D 
below 60: Grade F.

#include <stdio.h>
int main() 
{
    int percentage;
    printf("Enter percentage (0-100): ");
    scanf("%d", &percentage);
    if (percentage < 0 || percentage > 100) 
    {
        printf("Invalid percentage! Please enter between 0 and 100.\n");
    }
    else if (percentage >= 90) 
    {
        printf("Grade A\n");
    }
    else if (percentage >= 80)
    {
        printf("Grade B\n");
    }
    else if (percentage >= 70)
    {
        printf("Grade C\n");
    }
    else if (percentage >= 60) 
    {
        printf("Grade D\n");
    } else 
    { printf("Grade F\n"); }
     return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/53242ee9-d5a5-4fd6-b83b-1170ba17503c" />

Q19: Write a program to classify a triangle as Equilateral, Isosceles, or Scalene based on its side lengths.

#include <stdio.h>

int main() 
{
    int a, b, c;
    printf("Enter three sides of the triangle: ");
    scanf("%d %d %d", &a, &b, &c);
    if (a + b > c && a + c > b && b + c > a) 
    {
        if (a == b && b == c) 
        {
            printf("Equilateral\n");
        }
        else if (a == b || b == c || a == c) 
        {
            printf("Isosceles\n");
        }
        else
         {
            printf("Scalene\n");
        }
    } 
    else 
    {
        printf("Not a valid triangle\n");
    }
     return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/fed9a863-8c92-410d-bbc3-a6719a2fb041" />

Q20: Write a program to display the day of the week based on a number (1–7) using switch-case.

#include <stdio.h>
int main() {
    int day;
    printf("Enter a number (1-7): ");
    scanf("%d", &day);
    switch(day) {
        case 1:
            printf("Monday\n");
            break;
        case 2:
            printf("Tuesday\n");
            break;
        case 3:
            printf("Wednesday\n");
            break;
        case 4:
            printf("Thursday\n");
            break;
        case 5:
            printf("Friday\n");
            break;
        case 6:
            printf("Saturday\n");
            break;
        case 7:
            printf("Sunday\n");
            break;
        default:
            printf("Invalid input! Enter a number between 1 and 7.\n");
    }
     return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/c4133232-e6b7-4137-b5bb-7694dfe64f65" />

Q21: Write a program to display the month name and number of days using switch-case for a given month number.

#include <stdio.h>
int main() 
{
    int month;
    printf("Enter month number (1-12): ");
    scanf("%d", &month);
    switch(month) {
        case 1:
            printf("January, 31 days\n");
            break;
        case 2:
            printf("February, 28 days\n");
            break;
        case 3:
            printf("March, 31 days\n");
            break;
        case 4:
            printf("April, 30 days\n");
            break;
        case 5:
            printf("May, 31 days\n");
            break;
        case 6:
            printf("June, 30 days\n");
            break;
        case 7:
            printf("July, 31 days\n");
            break;
        case 8:
            printf("August, 31 days\n");
            break;
        case 9:
            printf("September, 30 days\n");
            break;
        case 10:
            printf("October, 31 days\n");
            break;
        case 11:
            printf("November, 30 days\n");
            break;
        case 12:
            printf("December, 31 days\n");
            break;
        default:
            printf("Invalid month number! Enter 1-12.\n");
    }
      return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/0ef95580-9367-4ffb-b3e5-590ea02caa00" />

Q22: Write a program to find profit or loss percentage given cost price and selling price.

#include <stdio.h>

int main() 
{
    float costPrice, sellingPrice, amount, percentage;
    printf("Enter Cost Price and Selling Price: ");
    scanf("%f %f", &costPrice, &sellingPrice);

    if (sellingPrice > costPrice) 
    {
        amount = sellingPrice - costPrice;
        percentage = (amount / costPrice) * 100;
        printf("Profit %.2f%%\n", percentage);
    } 
    else if (sellingPrice < costPrice) 
    {
        amount = costPrice - sellingPrice;
        percentage = (amount / costPrice) * 100;
        printf("Loss %.2f%%\n", percentage);
    } 
    else
    {
        printf("No Profit No Loss\n");
    }

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/3f43faac-8368-43d6-a28e-bdfe55109246" />

Q23: Write a program to calculate library fine based on late days as follows: 
First 5 days late: ₹2/day 
Next 5 days late: ₹4/day 
Next 20 days days late: ₹6/day 
More than 30 days: Membership Cancelled.

#include <stdio.h>
int main()
 {
    int days;
    int fine = 0;
    printf("Enter number of late days: ");
    scanf("%d", &days);

    if (days <= 5)
    {
        fine = days * 2;
        printf("Fine ₹%d\n", fine);
    } 
    else if (days <= 10) 
    {
        fine = 5 * 2 + (days - 5) * 4;
        printf("Fine ₹%d\n", fine);
    } 
    else if (days <= 30)
    {
        fine = 5 * 2 + 5 * 4 + (days - 10) * 6;
        printf("Fine ₹%d\n", fine);
    } 
    else {
        printf("Membership Cancelled\n");
    }
     return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/611d09e4-78b2-4bd4-863c-9fb4ebc29eaa" />

Q24: Write a program to calculate electricity bill based on units consumed with these rates: 
First 100 units at ₹5/unit 
Next 100 units at ₹7/unit 
Next 100 units at ₹10/unit 
Above at ₹12/unit

#include <stdio.h>
int main() 
{
    int units;
    int bill = 0;
    printf("Enter units consumed: ");
    scanf("%d", &units);

    if (units <= 100) 
    {
        bill = units * 5;
    } 
    else if (units <= 200) 
    {
        bill = 100 * 5 + (units - 100) * 7;
    } 
    else if (units <= 300) 
    {
        bill = 100 * 5 + 100 * 7 + (units - 200) * 10;
    } 
    else 
    {
        bill = 100 * 5 + 100 * 7 + 100 * 10 + (units - 300) * 12;
    }

    printf("Bill: ₹%d\n", bill);

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/854c4a9d-c767-44b5-adc4-7af673d1d3f9" />

Q25: Write a program to implement a basic calculator using switch-case for +, -, *, /, %.

#include <stdio.h>
int main() {
    int a, b;
    char op;
    printf("Enter two numbers and an operator (+, -, *, /, %%): ");
    scanf("%d %d %c", &a, &b, &op);
    switch(op) {
        case '+':
            printf("%d\n", a + b);
            break;
        case '-':
            printf("%d\n", a - b);
            break;
        case '*':
            printf("%d\n", a * b);
            break;
        case '/':
            if (b != 0)
                printf("%d\n", a / b);
            else
                printf("Error: Division by zero\n");
            break;
        case '%':
            if (b != 0)
                printf("%d\n", a % b);
            else
                printf("Error: Division by zero\n");
            break;
        default:
            printf("Invalid operator!\n");
    }
     return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/b0c9f896-85d8-48e9-8010-5e80e7a14af7" />

Q26: Write a program to print numbers from 1 to n.

#include <stdio.h>

int main()
 {
    int n, i;

    printf("Enter a number: ");
    scanf("%d", &n);

    for(i = 1; i <= n; i++)
    {
        printf("%d ", i);
    }
    printf("\n");

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/427ccaa4-ca46-472f-8a0d-5d79cb6cbc8b" />

Q27: Write a program to print the sum of the first n odd numbers.

#include <stdio.h>

int main()
 {
    int n, i, sum = 0;
    printf("Enter a number: ");
    scanf("%d", &n);

    for(i = 1; i <= 2*n; i += 2) 
    {
        sum += i;
    }

    printf("Sum of first %d odd numbers: %d\n", n, sum);

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/73504f3c-62cf-4922-9e91-c9ea70a67e04" />

Q28: Write a program to print the product of even numbers from 1 to n.

#include <stdio.h>
int main() 
{
    int n, i;
    long long product = 1; 
    printf("Enter a number: ");
    scanf("%d", &n);

    for(i = 2; i <= n; i += 2)
    {
        product *= i;
    }

    if(n < 2) 
    {
        printf("No even numbers to multiply.\n");
    } 
    else 
    {
        printf("Product of even numbers from 1 to %d: %lld\n", n, product);
    }

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/5af72d74-288c-49fb-be0f-855aebbf99bd" />

Q29: Write a program to calculate the factorial of a number.

#include <stdio.h>
int main() 
{
    int n, i;
    long long factorial = 1; 
    printf("Enter a number: ");
    scanf("%d", &n);

    if(n < 0)
    {
        printf("Factorial is not defined for negative numbers.\n");
        return 0;
    }
    for(i = 1; i <= n; i++) 
    {
        factorial *= i;
    }

    printf("Factorial of %d is %lld\n", n, factorial);

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/df129926-7f4c-4f4a-a8d7-c99eb48118d9" />

Q30: Write a program to reverse a given number.

#include <stdio.h>
int main()
 {
    int num, reversed = 0, remainder;
    printf("Enter a number: ");
    scanf("%d", &num);

    int original = num;
    if(num < 0)
    {
        num = -num; 
    }
     while(num != 0) 
    {
        remainder = num % 10;
        reversed = reversed * 10 + remainder;
        num /= 10;
    }

    if(original < 0)
    {
        reversed = -reversed;
    }
      printf("Reversed number: %d\n", reversed);

    return 0;
}

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/d4258142-c7cc-4be3-b7a1-0373deb09806" />





















