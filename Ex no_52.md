
## Task

# Write a function int max_of_four(int a, int b, int c, int d) which reads four arguments and returns the greatest of them.

## Note

There is not built in max function in C. Code that will be reused is often put in a separate function, e.g. int max(x, y) that returns the greater of the two values.

## Input Format

Input will contain four integers - a,b,c,d , one on each line.

## Output Format

Print the greatest of the four integers.
Note: I/O will be automatically handled.

AIM:

To write a program to calculate maximum function.

ALGORITHM:

Start.

Define a variables.

Write a program to calculate maximum function.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End.

PROGRAM:


#include<stdio.h>

int max(int x,int y)

{

    return x>y ? x:y;
}


int max_of_four(int a,int b,int c,int d)

{

    int large=max(max(a,b),max(c,d));
    
    return large;
}

int main()

{

    int a,b,c,d;
    
    scanf("%d %d %d %d",&a,&b,&c,&d);
    
    int large=max_of_four(a,b,c,d);
    
    printf("%d",large);
    
    return 0;
}


OUTPUT

![Screenshot 2025-05-26 172434](https://github.com/user-attachments/assets/a96afc57-1735-48c8-9c92-4ce731c8cb5e)

RESULT:

Thus, the program is executed and verified successfully.
