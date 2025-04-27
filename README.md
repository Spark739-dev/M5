EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
      #include <stdio.h>
      int main(){
         double num=23.65;
         double *ptr=&num;
         *ptr=25.0;
         printf("Modified value : %1.2f",num);
    }

## OUTPUT:
 	

![image](https://github.com/user-attachments/assets/5df84566-5669-409c-a1a0-61ca8d2c7fd8)










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
     #include <stdio.h>
     unsigned long long calculateproduct(int n) {
         if(n==1) {
         return 1;
       }
         else{
         return n*calculateproduct(n-1);
       }
    }
    int main() {
       int n=12;
       unsigned long long product;
       product=calculateproduct(n);
       printf("The product of first 12 naturl numbers = %d",product);
       return 0;
    }
## OUTPUT:
![image](https://github.com/user-attachments/assets/a6cfe39e-a22f-4f1c-90f9-dc68c7c6bfa5)
        		
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
     #include <stdio.h>
     int main() {
     int row,col;
     int i,j;
     scanf("%d %d",&row,&col);
     int a[row][col];
     for(i=0;i<row;i++) {
          for(j=0;j<col;j++) {
              scanf("%d",&a[i][j]);
        }
    }
    for(i=0;i<row;i++) {
          int sum=0;
          for(j=0;j<col;j++) {
              sum+=a[i][j];
          }
          printf("Sum of rows %d = %d\n",i+1,sum);
     }
      
    }


## OUTPUT

![image](https://github.com/user-attachments/assets/dd8014f8-520c-41ea-b1f8-56a344c0c31a)

 
 

 ## RESULT
 
Thus the C program to String process executed successfully
 

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
     #include <stdio.h>
     #include <string.h>
     int main(){
        char str[100];
        int nums_row,i,j,k,index=0;
        scanf("%s",str);
        scanf("%d",&nums_row);
        int len=strlen(str);
        int midpoint=nums_row-1;
        for(i=0;i<nums_row;i++) {
             for(j=0;j<nums_row;j++) {
                printf(" ");
        }
             for(k=0;k<=i;k++) {
                printf("%c ",str[index % len]);
                index++;
        }
         printf("\n");
      }
       return 0;
    }

 ## OUTPUT
![image](https://github.com/user-attachments/assets/9c0e8404-3875-430d-bcb5-9f65304a95d9)

 

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
     #include <stdio.h>
     int main() {
       int i,n;
       int arr[10];
       int *ptr=arr;
       scanf("%d",&n);
       for(i=0;i<n;i++) {
           scanf("%d",ptr+i);
     }
     printf("The elements are:\n");
     for(i=0;i<n;i++){
          printf("%d ",*(ptr+i));
      }
      printf("\n");
      return 0;
    }
    
## OUTPUT
![image](https://github.com/user-attachments/assets/7a37847f-ef32-4349-9e1e-3d20686cb7f4)

 

## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


