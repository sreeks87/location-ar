
# 🧮 Simple Calculator in Python – Step-by-Step Tutorial

### ✅ What you’ll learn in this tutorial:

* How to print messages
* How to take input from the user
* How to use `if` conditions to decide what the user wants to do
* How to use functions for each operation
* How to perform addition, subtraction, multiplication, and division

---
## 👣 Step 0: Make a new file called `calculator.py` in pycharm
####  To run the file use `python calculator.py` or use the play button at the top of pycharm



## 👣 Step 1: Print the calculator name

Let’s first make the program show the title of our calculator.

📄 **Code:**

```python
print("Simple Calculator")
```

📌 This line will simply show the name of our program. You can run just this to test.

---

## 👣 Step 2: Ask the user what operation they want

Use `input()` to ask the user to choose an operation: Add, Subtract, Multiply, or Divide.

📄 **Code:**

```python
print("What would you like to do?")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

choice = input("Enter the number of your choice (1/2/3/4): ")
```

📌 This lets the user type 1, 2, 3, or 4. We save that choice in a variable called `choice`.

---

## 👣 Step 3: Ask for two numbers

Now we need two numbers to perform the operation.

📄 **Code:**

```python
num1 = input("Enter the first number: ")
num2 = input("Enter the second number: ")
```

🧠 Wait! These are **strings** by default, so we need to convert them to **numbers** using `int()` (if your son knows only integers for now).

📄 **Update the code like this:**

```python
num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))
```

---

## 👣 Step 4: Create functions for each operation

Let’s create small functions to do each task. Functions help organize code.

📄 **Code:**

```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b
```

📌 These functions take two numbers (`a` and `b`) and return the result.

---

## 👣 Step 5: Use `if` conditions to run the correct operation

Now, based on what the user chose (1 to 4), we run the matching function.

📄 **Code:**

```python
if choice == "1":
    result = add(num1, num2)
    print("The answer is:", result)

elif choice == "2":
    result = subtract(num1, num2)
    print("The answer is:", result)

elif choice == "3":
    result = multiply(num1, num2)
    print("The answer is:", result)

elif choice == "4":
    result = divide(num1, num2)
    print("The answer is:", result)

else:
    print("Invalid choice. Please select 1, 2, 3, or 4.")
```

📌 This will match the user’s choice and perform the right operation.

---

## ✅ Final Code (Full Program)

Here’s how the full program looks when all parts are put together:

```python
# Print the title
print("Simple Calculator")

# Show options to the user
print("What would you like to do?")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

# Take user choice
choice = input("Enter the number of your choice (1/2/3/4): ")

# Ask for numbers
num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))

# Define functions
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b

# Perform the chosen operation
if choice == "1":
    result = add(num1, num2)
    print("The answer is:", result)

elif choice == "2":
    result = subtract(num1, num2)
    print("The answer is:", result)

elif choice == "3":
    result = multiply(num1, num2)
    print("The answer is:", result)

elif choice == "4":
    result = divide(num1, num2)
    print("The answer is:", result)

else:
    print("Invalid choice. Please select 1, 2, 3, or 4.")
```

---

## 🎉 What your son will learn by doing this:

* How to break a problem into steps
* How to use `input()` and `print()`
* How to write and use functions
* How to use `if-elif-else` for decisions
* How to work with variables and arithmetic

---
