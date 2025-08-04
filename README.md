# Simple Calculator Program

## Description

This is a straightforward Python program that allows a user to input two numbers and select a mathematical operation to perform on those numbers. The program supports addition (`+`), subtraction (`-`), multiplication (`*`), and division (`/`). It then displays the result of the computation.

## Features

- Accepts two numeric inputs (including decimals).
- Supports four basic operations: addition, subtraction, multiplication, and division.
- Handles division by zero gracefully, displaying an error message.
- Validates the operation input and notifies the user if an invalid operator is entered.

## How to Use

1. Run the Python script.
2. When prompted, enter the first number.
3. Enter the second number.
4. Enter the operation symbol (one of `+`, `-`, `*`, or `/`).
5. See the result displayed in the format:  
   `num1 operation num2 = result`

### Example

```
Enter the first number: 10
Enter the second number: 5
Enter the operation (+, -, *, /): +
10.0 + 5.0 = 15.0
```

## Notes

- Input must be a valid number (integers or floating-point numbers).
- Division by zero is not allowed and will prompt an error message.
- Operation input is case-sensitive and must be one of the four specified symbols.

## Requirements

- Python 3.x

## Code Snippet

```python
# Ask the user for the first number
num1 = float(input("Enter the first number: "))

# Ask the user for the second number
num2 = float(input("Enter the second number: "))

# Ask the user for the operation
operation = input("Enter the operation (+, -, *, /): ")

# Perform the operation and print the result
if operation == '+':
    result = num1 + num2
    print(f"{num1} + {num2} = {result}")
elif operation == '-':
    result = num1 - num2
    print(f"{num1} - {num2} = {result}")
elif operation == '*':
    result = num1 * num2
    print(f"{num1} * {num2} = {result}")
elif operation == '/':
    if num2 != 0:
        result = num1 / num2
        print(f"{num1} / {num2} = {result}")
    else:
        print("Error: Division by zero is not allowed.")
else:
    print("Invalid operation. Please enter +, -, *, or /.")
```

If you want, I can also help you add enhancements or features!
