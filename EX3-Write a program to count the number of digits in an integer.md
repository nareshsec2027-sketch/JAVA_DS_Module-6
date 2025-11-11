## EX 4: Nature of Resultant Matrix (Odd/Even/Mixed)

## DATE: 10.11.2025
## AIM:
To write a Java program to evaluate whether Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of the resultant matrix.

## Algorithm

Start the program.

Read dimensions and elements of Matrix A and B.

Add the matrices element-wise to form Matrix C.

Check each element in Matrix C:

If all elements are even → Resultant is Even Matrix.

If all are odd → Odd Matrix.

Otherwise → Mixed Matrix.

Display the result.

## Program
```
Program to find the nature of resultant matrix.
Developed by: Naresh P.S
RegisterNumber: 212223040127
Date: 10.11.2025

import java.util.*;
public class MatrixNature {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter rows and columns: ");
        int r = sc.nextInt(), c = sc.nextInt();

        int[][] A = new int[r][c];
        int[][] B = new int[r][c];
        int[][] C = new int[r][c];

        System.out.println("Enter Matrix A (odd numbers):");
        for (int i = 0; i < r; i++)
            for (int j = 0; j < c; j++)
                A[i][j] = sc.nextInt();

        System.out.println("Enter Matrix B (even numbers):");
        for (int i = 0; i < r; i++)
            for (int j = 0; j < c; j++)
                B[i][j] = sc.nextInt();

        boolean allEven = true, allOdd = true;

        System.out.println("Resultant Matrix C:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                C[i][j] = A[i][j] + B[i][j];
                System.out.print(C[i][j] + " ");
                if (C[i][j] % 2 == 0)
                    allOdd = false;
                else
                    allEven = false;
            }
            System.out.println();
        }

        if (allEven)
            System.out.println("Resultant Matrix is EVEN.");
        else if (allOdd)
            System.out.println("Resultant Matrix is ODD.");
        else
            System.out.println("Resultant Matrix is MIXED.");
    }
}
```
## Output
<img width="1918" height="789" alt="image" src="https://github.com/user-attachments/assets/2cfbb0ac-90af-4548-8dc2-9332b1eee26b" />


## Result

Thus, the Java program to find the nature of the resultant matrix is implemented successfully.
