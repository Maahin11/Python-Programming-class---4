# Python Code Examples

This repository contains a collection of Python code examples demonstrating various programming concepts and techniques. Below is a brief overview of the code snippets included in the notebook.

## Code Examples

### 1. **Iterating Over a String**
   - **Description**: This code iterates over each character in the string `"hello"` and prints each character on a new line.
   - **Code**:
     ```python
     word = "hello"
     for char in word:
         print(char)
     ```

### 2. **Dictionary Iteration**
   - **Description**: This code demonstrates how to iterate over the values and key-value pairs in a dictionary.
   - **Code**:
     ```python
     students_ages = {"Alice": 25, "Bob": 30, "Charlie": 35}
     for age in students_ages.values():
         print(age)
     for student, age in students_ages.items():
         print(student, age)
     ```

### 3. **Caesar Cipher Encryption**
   - **Description**: This code encrypts a message using the Caesar cipher technique by shifting each character by a specified key.
   - **Code**:
     ```python
     plaintext = input("Put a message: ")
     key = int(input("Put a key: "))
     cipher = ""
     for char in plaintext:
         cipher += chr(ord(char) + key)
         print(cipher)
     ```

### 4. **Caesar Cipher Decryption**
   - **Description**: This code decrypts a message encrypted with the Caesar cipher by shifting each character back by the specified key.
   - **Code**:
     ```python
     plaintext = input("Put a message: ")
     key = int(input("Put a key: "))
     cipher = ""
     for char in plaintext:
         cipher += chr(ord(char) - key)
         print(cipher)
     ```

### 5. **Zipping Lists**
   - **Description**: This code demonstrates how to use the `zip` function to iterate over two lists simultaneously.
   - **Code**:
     ```python
     names = ["Alice", "Bob", "Charlie"]
     ages = ['25', '30', '35']
     for name, age in zip(names, ages):
         print(name, age)
     ```

### 6. **Enumerating a List**
   - **Description**: This code uses the `enumerate` function to iterate over a list while keeping track of the index.
   - **Code**:
     ```python
     fruits = ["apple", "banana", "cherry"]
     for index, fruit in enumerate(fruits):
         print(index, fruit)
     ```

### 7. **Nested Loops**
   - **Description**: This code demonstrates nested loops by iterating over three ranges and printing the combination of indices.
   - **Code**:
     ```python
     for i in range(4):
         for j in range(3):
             for k in range(2):
                 print(i, j, k)
     ```

### 8. **Iterating Over a Matrix**
   - **Description**: This code iterates over a 2D list (matrix) and prints each element.
   - **Code**:
     ```python
     matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
     for row in matrix:
         for element in row:
             print(element)
     ```

### 9. **Finding Maximum and Minimum Values**
   - **Description**: These code snippets find the maximum and minimum values in a list.
   - **Code**:
     ```python
     A = [3, 41, 12, 9, 74, 15]
     max = A[0]
     for i in A:
         if i > max:
             max = i
     print(max)

     min = A[0]
     for i in A:
         if i < min:
             min = i
     print(min)
     ```

### 10. **Finding the Smallest Value**
   - **Description**: This code finds the smallest value in a list using a loop.
   - **Code**:
     ```python
     A = [3, 41, 12, 9, 74, 15]
     smallest = None
     for i in A:
         if smallest is None or i < smallest:
             smallest = i
     print("Smallest value:", smallest)
     ```

### 11. **Printing Numbers in a Range**
   - **Description**: This code prints numbers from 1 to 10 using a `for` loop.
   - **Code**:
     ```python
     for i in range(1, 11):
         print(i)
     ```

### 12. **Sum of Natural Numbers**
   - **Description**: This code calculates the sum of the first `n` natural numbers.
   - **Code**:
     ```python
     n = int(input("Enter a number: "))
     sum = 0
     for i in range(1, n + 1):
         sum += i
     print("Sum of first", n, "natural numbers is:", sum)
     ```

### 13. **Sum of Even Numbers**
   - **Description**: This code calculates the sum of the first `n` even numbers.
   - **Code**:
     ```python
     n = int(input("Enter a number: "))
     sum = 0
     for i in range(1, n + 2):
         sum += i
     print("Sum of first", n, "Even numbers is:", sum)
     ```

### 14. **Factorial Calculation**
   - **Description**: This code calculates the factorial of a number using a loop.
   - **Code**:
     ```python
     n = int(input("Enter a number: "))
     factorial = 1
     for i in range(1, n + 1):
         factorial *= i
         print(factorial)
     print("Factorial", n, "is:", factorial)
     ```

### 15. **Multiplication Table**
   - **Description**: This code prints the multiplication table for a given number.
   - **Code**:
     ```python
     n = int(input("Enter a number: "))
     for i in range(1, 11):
         print(f"{n} x {i} = {n * i}")
     ```

### 16. **Digit Frequency Counter**
   - **Description**: This code counts the frequency of each digit in a given number.
   - **Code**:
     ```python
     Digit = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     n = int(input("Enter a number: "))
     while n > 0:
         d = n % 10
         Digit[d] += 1
         n //= 10
     print(Digit)
     ```

### 17. **Prime Number Checker**
   - **Description**: This code checks if a given number is a prime number.
   - **Code**:
     ```python
     import math
     n = int(input("Enter a number: "))
     prime = True
     for i in range(2, int(math.sqrt(n)) + 1):
         if n % i == 0:
             prime = False
             break
     if prime:
         print(n, 'is a Prime number')
     else:
         print(n, 'is not a Prime number')
     ```

## How to Use
- Clone the repository or download the notebook file.
- Open the notebook in a Python environment (e.g., Jupyter Notebook, Google Colab).
- Run each cell to see the output of the code.

## Author
- **Md. Jubayerul Hasan Mahin**  
- **ID**: 213902127
