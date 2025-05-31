## print all the letters of the English alphabet.

SAMPLE OUTPUT : CAPS and add space to each alphabet

A B C D E F G H I J K L M N O P Q R S T U V W X Y Z

AIM:

To write a program to print all of the English alphabet'

ALGORITHM

1.Start: Initialize a loop that will iterate through the English alphabet.

2.Set Initial Character: Start with the first letter of the alphabet, 'a'.

3.Loop Through Characters: Use a loop to print each character, starting from 'a' and ending at 'z'.

4.Print Each Character: In each iteration, print the current character.

5.End: Once all characters have been printed, terminate the program.

Program

#include <stdio.h>

int main() 
{
    for(char c = 'A'; c <= 'Z'; c++) 
    {
        printf("%c ", c);
    }
    
    
    return 0;
}

Output

![Screenshot 2025-05-26 172933](https://github.com/user-attachments/assets/94b123f3-6425-4243-915b-e8c285dcb9c2)

Result

Thus, the program is executed and verified successfully.
