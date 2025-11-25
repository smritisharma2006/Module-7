# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:
```
def sum_digit(n):
    # Base Case
    if n <= 0:
        return 0
    # Recursive Case
    return (n % 10) + sum_digit(n // 10)

num = int(input("Enter a positive integer: "))
result = sum_digit(num)
print(f"Sum of digits of {num} is: {result}")
```
## OUTPUT
```
Enter a positive integer: 1234
Sum of digits of 1234 is: 10
````
## RESULT
Hence calculated the **sum of all digits** in a number using **recursion**
