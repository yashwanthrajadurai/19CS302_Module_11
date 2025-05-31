
# EX 51 C program to reverse a string.

## AIM:

To write a C program to reverse a string.

## Algorithm

.Initialize two pointers:


One pointer start at the beginning of the string (index 0).


Another pointer end at the last character of the string (index length - 1).


2.Loop through the string:

3.While start is less than end, swap the characters at the start and end positions.

Increment start and decrement end to move towards the middle of the string.

Terminate when start is no longer less than end.

4.Output the reversed string.  

## Program:

#include<stdio.h>

#include<string.h>

void reverseString(char str[]){

    int n=strlen(str);
    
    for(int i=0;i<n/2;i++){
    
        char temp=str[i];
        
        str[i]=str[n-i-1];
        
        str[n-i-1]=temp;
    }
    
}

int main(){

    char str[100];
    
    fgets(str,sizeof(str),stdin);
    
    printf("Input String: %s",str);
    
    str[strcspn(str, "\n")] = '\0';
    
    reverseString(str);
    
    printf("Reverse String: %s\n",str);
    
    return 0;

}

## Output:

![Screenshot 2025-05-26 172209](https://github.com/user-attachments/assets/e400e9b7-bc43-455d-8153-55eee1a3be6d)


## Result:

Thus the program was executed and the output was verified successfully.
