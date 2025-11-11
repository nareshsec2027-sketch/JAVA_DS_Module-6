## EX 5: Count Inversions in an Array

## DATE: 10.11.2025
## AIM:
To write a Java program to count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j.

## Algorithm

Start the program.

Read the array elements.

Use nested loops to count pairs (i, j) where arr[i] > arr[j] and i < j.

Display the count.

Stop the program.

## Program
```
Program to count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: Naresh P.S
RegisterNumber: 212223040127
Date: 10.11.2025

import java.util.*;
public class CountInversions {
    static int countInversions(int[] arr) {
        int count = 0;
        for (int i = 0; i < arr.length - 1; i++)
            for (int j = i + 1; j < arr.length; j++)
                if (arr[i] > arr[j])
                    count++;
        return count;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        System.out.println("Number of inversions: " + countInversions(arr));
    }
}
```

## Output
Enter number of elements: 5
Enter array elements:
2 4 1 3 5
Number of inversions: 3
<img width="1898" height="772" alt="image" src="https://github.com/user-attachments/assets/12b4f51e-01c1-4c91-ace0-74c56dd47bdd" />


## Result

Thus, the Java program to count the number of inversions in an array is implemented successfully.
