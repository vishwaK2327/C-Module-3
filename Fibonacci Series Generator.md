# # Fibonacci Series Generator

## 🧠 Aim

To write a program to generate the Fibonacci series for `n` numbers using a function that:
- Has no return type.
- Takes no arguments.

## 📋 Algorithm

1. Define a function `fib()` that calculates the Fibonacci series.
2. Inside `fib()`:
   - Read input value `n` from the user.
   - Initialize two variables: `a = 0`, `b = 1`.
   - Print the first two Fibonacci numbers: `a` and `b`.
   - Use a loop to generate and print the next `n-2` Fibonacci numbers.
3. In the `main()` function:
   - Call the `fib()` function.
   - Return 0 to indicate successful program termination.

## 🧾Program
```
#include <stdio.h>
void fib() {
    int n, i, a = 0, b = 1, c;
    printf("Enter the number of terms: ");
    scanf("%d", &n);
    if (n <= 0) {
        printf("Please enter a positive number.\n");
        return;
    }
    printf("Fibonacci Series: ");
    if (n >= 1)
        printf("%d ", a);
    if (n >= 2)
        printf("%d ", b);
    for (i = 3; i <= n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }
    printf("\n");
}
int main() {
    fib();  // Call the function
    return 0;
}
```

## Sample Output
```
Input:
Enter the number of terms: 7
Output:
Fibonacci Series: 0 1 1 2 3 5 8
```
## Result
The above programme is implemented and executed.
