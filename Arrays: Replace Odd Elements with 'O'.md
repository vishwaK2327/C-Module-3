# Arrays: Replace Odd Elements with 'O' in an Array

This repository contains a **C program** that reads a one-dimensional array of integers and **replaces all odd elements with the character `'O'`** when displaying the output.

## 🧠 Aim

To write a C program that replaces all odd elements of an array with `'O'`.

## 📋 Algorithm

1. Declare integer variables: `i`, `n` and an array `a[100]`.
2. Read the value of `n` (number of elements in the array) from the user.
3. Read `n` integers into the array `a`.
4. Loop through each element of the array:
   - If the element is odd (`a[i] % 2 != 0`), print `'O'`.
   - Otherwise, print the element itself.
5. Print each result separated by a space.

## 🧾Program
```
#include <stdio.h>
int main() {
    int a[100], n, i;
    // Step 2: Read number of elements
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }
    printf("Modified array output:\n");
    for (i = 0; i < n; i++) {
        if (a[i] % 2 != 0)
            printf("O ");
        else
            printf("%d ", a[i]);
    }
    printf("\n");
    return 0;
}
```

## Sample Output
```
Input:
Enter number of elements: 6
Enter 6 integers:
2 5 8 3 10 7
Output:
Modified array output:
2 O 8 O 10 O
```
## Result
The above programme is implemented and executed.
