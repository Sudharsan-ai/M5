EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
```
//Sudharsan S
//Reg no : 212224040334
#include <stdio.h>
int main() {
   double a = 23.65;
   double *ptr = &a;
   *ptr = 25.0;
   printf("Modified value: %.1f",a);
  
}
```

## OUTPUT:
 	
![image](https://github.com/user-attachments/assets/ae497319-f960-4802-b117-dea1ddf94655)


## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
```
// Sudharsan S
// Reg no : 212224040334
#include <stdio.h>

int natuprod(int n);

int main() {
    int n = 12;
    printf("Product of first %d natural numbers is: %d\n", n, natuprod(n));
}

int natuprod(int n) {
    if(n <= 1)
        return 1;
    else
        return n * natuprod(n - 1);
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/2f332fa1-24f3-4942-8e14-cf6cc23a0d0b)

          
## RESULT:

Thus the program has been executed successfully.
 

# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:
```
//Sudharsan S
 //Reg no : 212224040334 
#include <stdio.h>
int main() {
    int r,c;
    printf("Enter the number of rows: ");
    scanf("%d",&r);
    printf("\nEnter the number of columns: ");
    scanf(" %d",&c);
    int arr[r][c];
    printf("\n");
    for(int i=0;i<r;i++){
        printf("Enter the elements of Row %d: ",i+1);
        for(int j=0;j<c;j++){
            scanf("%d",&arr[i][j]);
        }
        printf("\n") ;
   
    }
    for(int i=0;i<r;i++){
        int sum = 0;
        for(int j=0;j<c;j++){
            sum += arr[i][j];
        }
        printf("The sum of the elements in Row %d is: %d \n\n",i+1,sum);
        
    }
    
}

```


## OUTPUT


 
 ![Uploading image.png…]()


 ## RESULT
 


# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:


 ## OUTPUT

 

## RESULT

Thus the C program to String process executed successfully
 

 
.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM

## OUTPUT

 

## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


