# EX-06 - Looping
## AIM:
Write a C program to print 1 to n numbers.

## ALGORITHM:
1.	Start.
2. Declare an integer variable a.
3. Read the value of a from the user input.
4. Initialize a loop counter i to 1.
5. Repeat the steps while i is less than or equal to a
6. Print the value of i.
7. Increment i by 1.
8. End.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for(int i=1;i<=a;i++)
    {
        printf("%d ",i);
    }
    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/5334328b-9d7c-4605-a8e3-c8c2f8a569ec)










## RESULT:
Thus the program to print 1 to n numbers has been executed successfully
 
 


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
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for(int i=a;i>0;i--)
    {
        for(int j=0;j<i;j++)
        {
            printf("#");
        }
        printf("\n");
        
    }
    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/c86c48b6-8bbe-4cde-b19f-ff3bc4cf2b79)




## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to add two numbers using auto storage class with return type & with arguments.

## ALGORITHM:

1. Start.
2. Declare two integer variables a and b.
3. Input two integers from the user and store them in a and b.
4. Call a function addi(a, b) 
5. Takes a and b as arguments.
6. Returns the sum of a and b.
7. Store the returned value into a variable c.
8. Print the value of c as the result of the addition.
9. End.

## PROGRAM:
```
#include<stdio.h>
int addi(int a,int b){
    return a+b;
}
int main()
{
    int auto a,b;
    scanf("%d%d",&a,&b);
    int c=addi(a,b);
    printf("The Result of Addition is:%d",c);
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/b6c2bf39-a009-4860-bb98-334ec562ef87)





## RESULT:

Thus the program to add two numbers using auto storage class with return type & with arguments has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program for the pascal's triangle pattern

## ALGORITHM:

1. Start.
2. Declare integer variables: row, i, j, c, and s.
3. Input the number of rows (row) from the user.
4. For each row number i from 0 to row - 1 
5. For spacing (s from 3 to row - i + 1):
6. Print a space " ".
7. Initialize a loop for columns (j from 0 to i):
8. If j == 0 or i == 0, then set c = 1.
9. c = c * (i - j + 1) / j
10. Print c followed by a space.
11. After printing all numbers in a row, move to the next line.
12. End.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int row,i,j,c,s;
    scanf("%d",&row);
    for(i=0;i<row;i++){
        for(s=3;s<=row-i+1;s++){
            printf(" ");
        }
        for(j=0;j<=i;j++){
            if(j==0||i==0)
            c=1;
            else
            c=c*(i-j+1)/j;
            printf("%d ",c);
        }
        printf("\n");
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/a30ca35a-264b-47c9-9c4a-92623bbd12be)




## RESULT:

Thus the program  for the pascal's triangle pattern has been executed successfully.




# EX – 10 - Fibonacci series Using a Function
## AIM:
To write a C program to generate Fibonacci series for given number using function without return type & without arguments.
## ALGORITHM:
1. Start.
2. Define a function fibo() that will:
3. Declare integers: n, i, a, b, and next.
4. Initialize a = 0, b = 1.
5. Input the value of n (number of terms to generate).
6. For each term i from 0 to n-1
7. Print the value of a.
8. Calculate next = a + b.
9. Update a = b.
10. Update b = next.
11. In main(), call the fibo() function.
12. End

## PROGRAM:
```
#include <stdio.h>
void fibo(){
    int n,i,a=0,b=1,next;
    scanf("%d",&n);
    for(i=0;i<n;i++){
        printf("%d ",a);
        next=a+b;
        a=b;
        b=next;
    }
}
int main(){
    fibo();
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/f549d0ec-a039-49ee-9f9e-3305ff1a2437)

## RESULT:
The program correctly computes to generate Fibonacci series for given number using function without return type & without arguments displays the result.
 
