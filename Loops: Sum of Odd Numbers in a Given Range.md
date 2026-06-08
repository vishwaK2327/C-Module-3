# Loops: Sum of Odd Numbers in a Given Range

This project contains a simple **C program** that calculates the **sum of all odd numbers** within a user-defined range using a **`for` loop**.

## 🧠 Aim

To write a C program that finds and sums all odd numbers in a specified range using a `for` loop.

## 📋 Algorithm

1. Declare integer variables: `n`, `m`, `i`, and `sum`. Initialize `sum = 0`.
2. Prompt the user to enter the starting (`m`) and ending (`n`) values of the range.
3. Use a `for` loop to iterate from `m` to `n - 1`.
4. Inside the loop:
   - Check if the current number `i` is odd (`i % 2 != 0`).
   - If odd, print `i` and add it to `sum`.
5. After the loop, display the total `sum` of the odd numbers.
6. Return `0` to indicate successful execution.

## 💻 Program
```
#include <stdio.h>
int main() {
    int m, n, i, sum = 0;
    printf("Enter the starting value of the range (m): ");
    scanf("%d", &m);
    printf("Enter the ending value of the range (n): ");
    scanf("%d", &n);
    printf("Odd numbers between %d and %d are:\n", m, n);
    for (i = m; i < n; i++) {
        if (i % 2 != 0) {
            printf("%d ", i);
            sum += i;
        }
    }
    printf("\nSum of odd numbers in the range: %d\n", sum);
    return 0;
}
```

## Output
```
Input:
Enter the starting value of the range (m): 5
Enter the ending value of the range (n): 15
Output:
Odd numbers between 5 and 15 are:
5 7 9 11 13 
Sum of odd numbers in the range: 45
```
## Result
The above programme is implemented and executed.
