# EX-11-EMI-CALCULATOR

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
#include <stdio.h>
#include<math.h>
void calculateEMI(float principal, float annualRate, int years) {
    float monthlyRate = annualRate / (12 * 100);
    int months = years * 12;
    float emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);

    printf("Monthly EMI is= %.3f\n", emi);
}

int main() {
    float principal;
    float rate ;
    int years ;
    scanf("%f", &principal);
    scanf("%f", &rate);
    scanf("%d", &years);

    calculateEMI(principal, rate, years);

    return 0;
}
```

## OUTPUT


![Screenshot 2025-05-22 103735](https://github.com/user-attachments/assets/80204b6d-b3a1-4615-b669-64d53c547123)



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
void generateFibonacci(int n)
{
    int a = 0, b = 1, next;
    for (int i=0; i<n; i++) {
        printf("%d ", a);
        next = a + b;
        a=b;
        b=next;
    }
    printf("\n");
}
int main()
{
    int number;
    scanf("%d", &number);
    generateFibonacci(number);
    return 0;
}
```

## OUTPUT



![Screenshot 2025-05-22 104048](https://github.com/user-attachments/assets/4d23053c-b50f-4b33-85c0-f6ae6b0d989f)




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
#include <stdio.h>

int main()
{
    int n;
    scanf("%d",&n);
    int arr[n];
    for(int i=0; i<n; i++)
    {
        scanf("%d", &arr[i]);
}
        printf("%d ",arr[n-1]);

    return 0;
}
```
## OUTPUT




![Screenshot 2025-05-22 104447](https://github.com/user-attachments/assets/c6d85e17-c522-44a8-ac5b-5d15aa8d1b77)






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
#include <stdio.h>
int main() {
    int arr[100], n, count = 0;
    scanf("%d", &n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(int i = 0; i < n; i++) {
        if (arr[i] >  0) {
            count++;
        }
    }

    printf("Positive numbers: %d\n", count);

    return 0;
}
```
## OUTPUT


![Screenshot 2025-05-22 105342](https://github.com/user-attachments/assets/84c33e86-9e03-4c2b-9fcf-cded9281ca63)



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
#include <stdio.h>
int main()
{
    int arr[100], n;
    scanf("%d", &n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Array after replacing even elements with 'E':\n");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");  
        } else {
            printf("%d ", arr[i]);  
        }
    }

    printf("\n");
    return 0;
}
```
## Output:
 
![Screenshot 2025-05-22 105632](https://github.com/user-attachments/assets/625974c9-2eef-4db9-a3ea-1be50ec6ae1d)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



