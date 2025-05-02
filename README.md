# EX-11-EMI-CALCULATOR

## AIM

write a program to prepare EMI calculator using function with return type with arguments.

## ALGORITHM

1.      Define a function calculate_EMI that takes principal (p), interest rate (r), and time in years (t) to calculate the EMI.
2.      In the EMI formula, convert the annual interest rate to a monthly rate and time to months.
3.      Use the formula to calculate EMI:- emi = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
4.      In the main function, take user input for principal amount, annual interest rate, and loan period in years.
5.      Call the function, store the result in emi, and print the monthly EMI amount.


## PROGRAM
```
#include <math.h>
#include <stdio.h>
// Function to calculate EMI
float calculate_EMI(float p, float r, float t){
   float emi;
   r = r / (12 * 100); // one month interest
   t = t * 12; // one month period
   emi = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
   return (emi);
}
int main(){
   float principle, rate, time1, emi;
   scanf("%f %f %f",&principle,&rate,&time1);
   emi = calculate_EMI(principle, rate, time1);
   printf("Monthly EMI is= %.3f", emi);
   return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/dfea1379-684a-4d8e-9a84-215549d07aee)





## RESULT

Thus the program to prepare EMI calculator using function with return type with arguments has been executed successfully.
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the given input.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    int x,f,a,b,i;
    scanf("%d ",&x);
    a=0;
    printf("%d ",a);
    
    b=1;
    printf("%d ",b);
    for(i=3;i<=x;i++)
    {
        f=a+b;
        printf("%d ",f);
        a=b;
        b=f;
    }
    return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/7b6ab660-0fdd-412c-85cc-d9aad4ed1381)






## RESULT
Thus the program to generate the Fibonacci series for the given input has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and to print the second last element of the array (integer).

## ALGORITHM

1.      Start the program and declare an integer n to store the number of elements.

2.      Take input from the user for n, then declare an integer array a of size n.

3.      Use a loop to read n elements from the user and store them in the array.

4.      Print the second last element of the array using a[n-2].

5.      End the program by returning 0.


## PROGRAM
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("%d",a[n-2]);
    return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/f2966f55-0feb-486d-b143-4dd2c37e581a)







## RESULT
Thus the program to read n elements as input and print the second last element of the array has been executed successfully.
 
 


# EX-14-EVEN-ARRAY-ELEMENTS
## AIM
Write a C Program to Print the Number of  Even Numbers in an Array

## ALGORITHM

1.      Start the program and declare an integer n to store the number of elements.

2.      Take input from the user for n, then declare an array a of size n.

3.      Use a loop to read n numbers from the user and store them in the array.

4.      Loop through the array again and check each number to see if it's even (a[i] % 2 == 0).

5.      Print all even numbers found in the array.



## PROGRAM
```
#include <stdio.h>
int main()
{
    int i,n;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("Even numbers in the array are - ");
    for(i=0;i<n;i++)
    {
        if(a[i]%2==0)
        {
            printf("%d ",a[i]);
        }
    }
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/4aaa2c00-62a0-4d69-bd61-8453ae30b458)



## RESULT
Thus the program to Print the Number of  Even Numbers in an Array  has been executed successfully.





 
 


# EX -15 - Replace All Odd Elements With '1' In One Dimensional Array

## Aim:
 To write a C program to replace all odd elements by 1 in one dimensional array

## Algorithm:

1.      Start the program and read an integer n from the user to determine the size of the array.

2.      Declare an array arr of size n and take n integer inputs from the user to fill it.

3.      Go through each element in the array using a loop.

4.      Check if each number is odd or even.

5.      If the number is even, keep it as it is.

6.      If the number is odd, replace it with 1.

7.      Print the updated array, where all odd numbers are now replaced by 1.


## Program:
```
#include <stdio.h>


int main() {
   
    int n;
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++)
    { 
        scanf("%d",&arr[i]);
        
    }
    
    for(int i=0;i<n;i++)
    { 
        
        if(arr[i]%2==0) arr[i]=arr[i];
        else arr[i]=1;
    }
    for(int i=0;i<n;i++)
        printf("%d ",arr[i]);
    
    
    return 0;
}
```
## Output:
 
![image](https://github.com/user-attachments/assets/425af290-5012-457a-a3a3-db3ecacfe5da)







## Result:

Thus, the program to replace all odd elements with '1' in one dimensional array was verified successfully.



