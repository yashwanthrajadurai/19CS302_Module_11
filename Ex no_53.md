# EX 53 C program to remove duplicates in an array.

## AIM:

To write a C program to remove duplicates in an array.

## Algorithm

1.Start: Begin with the given array of elements.

2.Loop Through Array: Iterate through each element of the array starting from the first.

3.Check for Duplicates: For each element, check if it already exists in the portion of the array that comes before it.

Use a nested loop to check if the current element matches any earlier element in the array.

4.Remove Duplicate: If a duplicate is found, shift all the subsequent elements one position to the left to remove the duplicate.

5.End: Once the array is traversed, the remaining elements in the array will be unique. The array is now free of duplicates.

## Program:

#include <stdio.h>


void removeDuplicates(int arr[], int *size) {

    int i, j, k;
    
    for (i = 0; i < *size; i++) {
    
        // Check for duplicates of arr[i]
        
        for (j = i + 1; j < *size; j++) {
        
            if (arr[i] == arr[j]) {
            
                // Shift elements to left after a duplicate is found
                
                for (k = j; k < *size - 1; k++) {
                
                    arr[k] = arr[k + 1];
                }
                
                
                (*size)--;  // Decrease array size
                
                j--;  // To check the new element at position j
           
            }
            
        }
    }
}

int main() {
    
    int arr[] = {10, 20, 10, 30, 20, 40, 30};
    
    int size = sizeof(arr) / sizeof(arr[0]);

    
    printf("Original array: ");
    
    for (int i = 0; i < size; i++) {
    
        printf("%d ", arr[i]);
   
    }
    
    printf("\n");
    
    removeDuplicates(arr, &size);
    
    printf("Array after removing duplicates: ");
    
    for (int i = 0; i < size; i++) {
    
        printf("%d ", arr[i]);
    }
    
    
    printf("\n");
    
    return 0;
}



## Output:

![Screenshot 2025-05-26 172655](https://github.com/user-attachments/assets/46a0f9a2-5787-4b22-b5b2-785c3b7f17df)


## Result:

Thus the program was executed and the output was verified successfully.
