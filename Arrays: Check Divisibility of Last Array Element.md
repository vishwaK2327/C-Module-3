# Arrays: Check Divisibility of Last Array Element

This repository contains a simple **C program** that reads `n` elements into an array and checks whether the **last element** is divisible by 2.

## 🧠 Aim

To create a C program that reads `n` integers into an array and determines if the **last element** is divisible by 2.

## 📋 Algorithm

1. Declare variables `n`, `i`, and an integer array `a[10]`.
2. Prompt the user to enter the value of `n` (number of elements).
3. Prompt: "The last element".
4. Read `n` elements into the array `a`.
5. Print the last element of the array.
6. Check if the last element (`a[n-1]`) is divisible by 2:
   - If true, print a message indicating it is divisible.
   - Otherwise, print a message that it is not divisible.
7. Return `0` to indicate successful execution.

## 🧾 Program
```
#include <stdio.h>
int main() {
    int n, i;
    int a[10];
    printf("Enter the number of elements (max 10): ");
    scanf("%d", &n);

  if (n > 10 || n <= 0) {
        printf("Invalid input. Please enter a value between 1 and 10.\n");
        return 1;
    }
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }
    printf("The last element is: %d\n", a[n - 1]);
    if (a[n - 1] % 2 == 0) {
        printf("The last element is divisible by 2.\n");
    } else {
        printf("The last element is not divisible by 2.\n");
    }
    return 0;
}
```

## Sample Output
```
User Input:
Enter the number of elements (max 10): 5
Enter 5 elements:
10
15
7
8
12
Program Output:
The last element is: 12
The last element is divisible by 2.
```

## Result
The above programme is implemented and executed.
