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
#include <math.h>


void calculateEMI(float principal, float rate, int time) {
    float emi;
    float monthlyRate = rate / (12 * 100); 
    int months = time * 12;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);

    printf("\nThe EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int time;

    
    scanf("%f", &principal);

   
    scanf("%f", &rate);

    
    scanf("%d", &time);

 
    calculateEMI(principal, rate, time);

    return 0;
}
```

## OUTPUT


![437940957-d15b6f9d-3da0-41ff-a814-e3ad3063745f](https://github.com/user-attachments/assets/b0b801a3-fa35-43be-9989-e591b1d414ef)



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
#include <stdio.h>

int main() {
    int n = 6; // Number of terms
    int first = 0, second = 1, next, i;

    printf("Fibonacci Series up to %d terms:\n", n);

    for (i = 0; i < n; i++) {
        if (i <= 1)
            next = i;
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }

    return 0;
}
```
## OUTPUT



![437941008-cdc27f77-0a25-4bf3-8a0e-7ef322435607](https://github.com/user-attachments/assets/362fa20a-bc49-4efd-992d-74fbac3de447)





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

int main() {
    int n, i;
;
    scanf("%d", &n);

    int arr[n]; 

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }


    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
```

## OUTPUT




![437941082-34851039-ad90-4502-b85c-dc0c5777a8a6](https://github.com/user-attachments/assets/ed29390e-9e3c-4e46-89f2-5effc431805b)





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
    int n, i, count = 0;


    scanf("%d", &n);

    int arr[n]; 

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        if (arr[i] > 0) {
            count++; 
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```

## OUTPUT



![437941144-cfca22c6-72b5-45c1-bfa6-52d15c754121](https://github.com/user-attachments/assets/fdd174ae-5db6-4cd7-921b-69980346c39b)




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

int main() {
    int n, i;

    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Array after replacing even elements with 'E':\n");
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    return 0;
}
```

## Output:


![437946698-8069572d-0579-4e34-acf8-50030e3aea5f](https://github.com/user-attachments/assets/71f65d08-f01a-4b32-b75c-d176582c3c4a)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



