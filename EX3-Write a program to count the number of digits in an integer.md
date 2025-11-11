## EX 3: Count Number of Digits in an Integer

## DATE: 10.11.2025
## AIM:
To write a Java program to count the number of digits in an integer using recursion.

## Algorithm

Start the program.

Read the integer input.

Define a recursive function countDigits(num):

Base case: If num == 0, return 0.

Else, return 1 + countDigits(num / 10).

Display the result.

Stop the program.

## Program
```
Program to count the number of digits in an integer.
Developed by: Naresh P.S
RegisterNumber: 212223040127
Date: 10.11.2025

import java.util.*;
public class CountDigits {
    static int countDigits(int num) {
        if (num == 0)
            return 0;
        return 1 + countDigits(num / 10);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int num = sc.nextInt();

        int count = countDigits(num);
        System.out.println("Number of digits: " + count);
    }
}
```

## Output
<img width="1919" height="780" alt="image" src="https://github.com/user-attachments/assets/b2c81755-76ff-4a99-962e-f6e05bd67c6e" />


## Result

Thus, the Java program to count the number of digits in an integer is implemented successfully.
