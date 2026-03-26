# EX-11-EMI-CALCULATOR

## NAME: R . NITHISH AADITIYAA

## REGISTER NO: 25011876 [ 212225040287 ]

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
#include<math.h>
void test(float principal,float rate,float year)
{
    float emi,n,m;
    rate=rate/(12*100);
    year=year*12;
    n=pow(1+rate,year);
    m=pow(1+rate,year)-1;
    emi=(principal*rate*n)/m;
    printf("Monthly EMI is= %.3f",emi);
    return ;
}
int main()
{
    float principal,rate,year;
    scanf("%f %f %f",&principal,&rate,&year);
    test(principal,rate,year);
    return 0;
}
```
## OUTPUT

![alt text](emi.png)

## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 

# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

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
    int N;
    scanf("%d",&N);
    printf("0 1 ");
    N=N-2;
    int N1=0,N2=1,temp;
    for(int i=1;i<=N;i++)
    {
        temp=N1;
        N1=N2;
        N2=N2+temp;
        printf("%d ",N2);
    }
    return 0;
}
```
## OUTPUT

![alt text](<Fibonacci series.png>)

## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 
# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    int n,count=0;
    scanf("%d",&n);
    int arr[n];
    for(int itr=0;itr<n;itr++)
    {
        scanf("%d",&arr[itr]);
    }
    printf("Last element: %d",arr[n-1]);
    return 0;
}
```
## OUTPUT

![alt text](array.png)

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 
# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    int n,count=0;
    scanf("%d",&n);
    int arr[n];
    for(int itr=0;itr<n;itr++)
    {
        scanf("%d",&arr[itr]);
    }
    for(int itr=0;itr<n;itr++)
    {
        if(arr[itr]>0)
        {
            count+=1;
        }
    }
    printf("The total no of positive elements: %d",count);
    return 0;
}
```
## OUTPUT

![alt text](<positive array.png>)

## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    int arr[100];
    for(int itr=0;itr<n;itr++)
    {
        scanf("%d",&arr[itr]);
    }
    printf("After replacing even elements with E:");
    for(int itr=0;itr<n;itr++)
    {
        if(arr[itr]%2==0)
        {
            printf("E ");
        }
        else
        {
            printf("%d ",arr[itr]);
        }
    }
    return 0;
}
```
## Output:

![alt text](<1 D array.png>)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



