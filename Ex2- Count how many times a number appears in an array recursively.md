## EX 2: Count How Many Times a Number Appears in an Array Recursively

## DATE: 10.11.2025
## AIM:
To write a Java program to count how many times a number appears in an array recursively.

## Algorithm

Start the program.

Read the array elements and the target number.

Define a recursive function countOccurrences(arr, n, x):

Base case: If n == 0, return 0.

If arr[n-1] == x, return 1 + countOccurrences(arr, n-1, x).

Else, return countOccurrences(arr, n-1, x).

Display the count.

Stop the program.

## Program
```
Program to count how many times a number appears in an array recursively.
Developed by: Naresh P.S
RegisterNumber: 212223040127
Date: 10.11.2025

import java.util.*;
public class CountOccurrences {
    static int countOccurrences(int[] arr, int n, int x) {
        if (n == 0)
            return 0;
        if (arr[n - 1] == x)
            return 1 + countOccurrences(arr, n - 1, x);
        else
            return countOccurrences(arr, n - 1, x);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        System.out.print("Enter number to count: ");
        int x = sc.nextInt();

        int count = countOccurrences(arr, n, x);
        System.out.println(x + " appears " + count + " times in the array.");
    }
}
```

## Output
<img width="1919" height="750" alt="image" src="https://github.com/user-attachments/assets/1dd5d5fd-20f7-471b-b552-105c177b0134" />

## Result

Thus, the Java program to count how many times a number appears in an array recursively is implemented successfully.
