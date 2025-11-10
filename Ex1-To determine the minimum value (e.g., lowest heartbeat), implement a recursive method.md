### EX 1: Find the Minimum Value (Lowest Heartbeat) Using Recursion
```
DATE: 10.11.2025
```
AIM:
```
To write a Java program to determine the minimum value (e.g., lowest heartbeat) using a recursive method.
```

Algorithm:
```
1.Start the program.
2.Read the array elements.
3.Define a recursive function findMin(arr, n):
4.Base case: If array size is 1, return the element.
5.Recursive case: Return the smaller value between arr[n-1] and findMin(arr, n-1).
6.Display the result.
7.Stop the program.
```

Program:
```
Program to determine the minimum value (e.g., lowest heartbeat) using recursion.
Developed by: Naresh P.S
RegisterNumber: 212223040127
Date: 10.11.2025
```

```
import java.util.*;

public class MinValueRecursion {
    static int findMin(int[] arr, int n) {
        if (n == 1)
            return arr[0];
        return Math.min(arr[n - 1], findMin(arr, n - 1));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of readings: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter the readings:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        int minValue = findMin(arr, n);
        System.out.println("Lowest heartbeat (Minimum Value): " + minValue);
    }
}
```
Output:
<img width="1915" height="774" alt="image" src="https://github.com/user-attachments/assets/d534802a-1301-45f6-b283-b5d84d8fc5b1" />


Result:

Thus, the Java program to determine the minimum value (e.g., lowest heartbeat) using recursion is implemented successfully.
