# EX 55 C program to find a square of number using function with arguments without return type.

## AIM:

To write a C program to find a square of number using function with arguments without return type.

## Algorithm

Start.

Define a variables.

Write a program to square of the given number.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End 

## Program:

#include <stdio.h>

int square(int num) {

 return num * num;

}

int main() {

 int number, result;
 
 scanf("%d", &number);
 
 result = square(number); // Function call
 
 printf("Square of %d is %d\n", number, result);

}


## Output:

![Screenshot 2025-05-26 173223](https://github.com/user-attachments/assets/27cd1c45-636f-4d51-8a2d-c3846451e55c)



## Result:

Thus the program was executed and the output was verified successfully.
