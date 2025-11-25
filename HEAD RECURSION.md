# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:
```
def sum_of_digits(num):
    """Helper function to calculate sum of digits of a number."""
    return sum(int(digit) for digit in str(num))

def fun(n):
    if n <= 0:
        return
    fun(n - 1)
    print(f"Current value: {n}, Sum of digits: {sum_of_digits(n)}")


num = int(input("Enter a positive integer: "))

if num % 2 != 0:
    num += 1

print(f"Adjusted input (even number): {num}\nSequence (head recursion):")
fun(num)
```

## OUTPUT
```
Enter a positive integer: 5
Adjusted input (even number): 6
Sequence (head recursion):
Current value: 1, Sum of digits: 1
Current value: 2, Sum of digits: 2
Current value: 3, Sum of digits: 3
Current value: 4, Sum of digits: 4
Current value: 5, Sum of digits: 5
Current value: 6, Sum of digits: 6
```
## RESULT
Hence  demonstrated **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).
