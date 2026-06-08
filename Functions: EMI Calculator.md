# Fuctions: EMI Calculator in C (Function Without Return Type With Arguments)

This repository contains a **C program** to calculate the **Equated Monthly Installment (EMI)** using a function that has **no return type but accepts arguments**.

## 🎯 Aim

To write a C program that calculates the EMI for a loan using a function **without return type and with arguments**.

## 📋 Algorithm

1. Start the program.
2. Read input values from the user:
   - Principal amount (`p`)
   - Rate of interest (`r`)
   - Loan duration in months (`t`)
3. Pass these values as arguments to a function.
4. Inside the function, calculate the EMI using the formula:
5. EMI = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1)

 Note: Ensure the rate `r` is converted to a monthly rate (i.e., divide annual rate by 12 * 100).

5. Display the EMI result.
6. Stop the program.

## 🧾Program
```
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float annualRate, int timeMonths) {
    float monthlyRate = annualRate / (12 * 100);  
    float emi;
    emi = (principal * monthlyRate * pow(1 + monthlyRate, timeMonths)) /
          (pow(1 + monthlyRate, timeMonths) - 1);
    printf("The EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int time;
    printf("Enter principal amount: ");
    scanf("%f", &principal);
    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &rate);
    printf("Enter loan duration in months: ");
    scanf("%d", &time);
    calculateEMI(principal, rate, time);
    return 0;
}
```
## Sample Output
```
Input:
Enter principal amount: 500000
Enter annual interest rate (in %): 7.5
Enter loan duration in months: 60
Output:
The EMI is: 10018.97
```
## Result
The above programme is implemented and executed.
