# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>

int main() {
  int m,n;
  printf("Enter the numbers: ");
  scanf("%d %d",&m,&n);
  for(int i=m;i<=n;i++)
  {
      if(i%2==0)
      printf("%d ",i);
  }
    return 0;
}
```
## OUTPUT:
<img width="1411" height="447" alt="image" src="https://github.com/user-attachments/assets/63071bca-77f7-4728-8233-3990adca4638" />










## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>

int main() {
  int rows;
  printf("Enter the number of rows to get printed: ");
  scanf("%d",&rows);
  for(int i=1;i<=rows;i++)
  {
      for(int space=1;space<=rows-i;space++)
      {
          printf(" ");
      }
      for(int k=1;k<=i;k++)
      {
          printf("* ");
      }
      printf("\n");
  }
  return 0;
}
```

## OUTPUT:
<img width="1528" height="631" alt="image" src="https://github.com/user-attachments/assets/4aa11719-9544-44a7-9ad4-c6a113d21ef7" />





## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>
void add(int a,int b)
{
    printf("Addition of two numbers is %d\n",a+b);
}
void subtract(int c,int d)
{
    printf("Subtraction of two numbers is %d",c-d);
}
int main() {
  int num1,num2;
  printf("Enter the first number: ");
  scanf("%d",&num1);
  printf("Enter the second number: ");
  scanf("%d",&num2);
  add(num1,num2);
  subtract(num1,num2);
  return 0;
}
```

## OUTPUT:
<img width="1463" height="611" alt="image" src="https://github.com/user-attachments/assets/40d12468-a95e-4c33-8eae-92948c1c549c" />






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    int n;
    int sum=0;
    printf("Enter a number: ");
    scanf("%d",&n);
    for(int i=n;i>0;i/=10)
    {
        int a=i%10;
        if(a%2!=0)
        sum+=a;
    }
    printf("Sum of odd digits are %d",sum);
    return 0;
    }
```

## OUTPUT:
<img width="1407" height="532" alt="image" src="https://github.com/user-attachments/assets/bf53392b-24b8-4d50-92d0-6f5dc1ba53ff" />




## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
int fact(int n)
{
    int fac=1;
    printf("Enter the number: ");
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
    {
        fac*=i;
    }
    printf("Factorial of %d is %d",n,fac);
}
int main()
{
    int n;
    fact(n);
    return 0;
}
```

## OUTPUT:
<img width="1312" height="579" alt="image" src="https://github.com/user-attachments/assets/4d97f0f4-510b-4e70-b1fb-656b2ed64adc" />

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
