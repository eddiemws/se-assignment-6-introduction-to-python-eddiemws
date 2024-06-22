[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15314708&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
Python is a high-level, interpreted programming language known for its simplicity and readability. Key features include:

Ease of Learning and Readability: Python's syntax resembles natural language, making it accessible for beginners and easy to read for experienced developers.
Versatility: Python supports multiple programming paradigms (procedural, object-oriented, functional) and is suitable for a wide range of applications.
Rich Standard Library: Python comes with a comprehensive standard library, providing modules and packages for tasks such as web development, data analysis, and more.
Community Support: A large community contributes libraries and frameworks, fostering rapid development.
Examples of Use Cases:

Web Development: Django and Flask are popular frameworks for building web applications.
Data Analysis and Machine Learning: Libraries like Pandas, NumPy, and scikit-learn are widely used in data science.
Scripting and Automation: Python is used for scripting tasks and automating repetitive processes.
Prototyping: Due to its rapid development capabilities, Python is ideal for prototyping new software products.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
     Windows:

Download the latest Python installer from python.org.
Run the installer, ensuring to check "Add Python to PATH" during installation.
Open Command Prompt or PowerShell and verify Python installation with python --version.
macOS:

macOS typically comes with Python pre-installed. You can verify and optionally install a newer version using Homebrew:
brew install python
python3 --version

Linux:
Use the package manager (e.g., apt, yum, dnf) to install Python:
sudo apt install python3
python3 --version
Setting up a Virtual Environment:

Install virtualenv using pip
pip install virtualenv

Create a virtual environment:
python -m venv myenv

Activate the virtual environment:
Windows: myenv\Scripts\activate
macOS/Linux: source myenv/bin/activate


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
     
# Simple Python program to print "Hello, World!"
print("Hello, World!")

Explanation:
print(): Function in Python used to output text to the console.
"Hello, World!": String literal enclosed in double quotes, which is the text to be printed.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
     
Basic Data Types:
Integer (int): Whole numbers without decimal points (e.g., 5, -3).
Float (float): Numbers with decimal points (e.g., 3.14, -0.5).
String (str): Sequence of characters enclosed in quotes (e.g., "Python", 'Hello').
Boolean (bool): Represents True or False values.

# Python script demonstrating data types and variables
# Integer
num1 = 100000
# Float
num2 = 123.678
# String
message = "Hello, World!"
# Boolean
is_true = True

# Printing variables
print(num1)
print(num2)
print(message)
print(is_true)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
Conditional Statement (if-else):

# Example of if-else statement
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
    
Loop (for loop):

# Example of for loop
# Iterating over a list
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
     
Functions are reusable blocks of code that perform a specific task. They promote code reusability and organization.

# Example of a function that returns the sum of two numbers
def sum_numbers(a, b):
    return a + b

# Calling the function
result = sum_numbers(3, 5)
print("Sum:", result)  # Output: Sum: 8


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
     
Lists: Ordered collections of items, accessed by numerical indexes starting from 0. They can contain duplicates and elements of any data type.
Dictionaries: Unordered collections of key-value pairs. Keys must be unique and immutable (like strings, numbers, or tuples). Values can be of any data type.

# Create a list of numbers
numbers = [1, 3, 5, 7, 9]

# Create a dictionary with key-value pairs
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}

# Basic operations on lists:
print("Second element in the list:", numbers[1])  # Access by index
numbers.append(11)  # Add an element (mutable)
numbers.remove(5)    # Remove an element (mutable)

# Basic operations on dictionaries:
print("Alice's age:", person["age"])   # Access by key
person["city"] = "Los Angeles"      # Modify a value (mutable)
# person["age"] = "thirty" (Invalid: keys must be immutable)

# Print the list and dictionary
print("List:", numbers)
print("Dictionary:", person)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   - 
 Exception Handling: A mechanism to catch and handle errors that might occur during program execution, preventing unexpected crashes.
try block: Contains code that might raise an exception.
except block: Executes if an exception is raised in the try block.
finally block: Executes regardless of whether an exception occurs (optional).
Example:
def divide(a, b):
    try:
        return a / b
    except ZeroDivisionError:
        print("Error: Cannot divide by zero")
        return None
    finally:
        print("Division operation completed")

result = divide(10, 2)
print("Result:", result)

result = divide(10, 0)  # Exception will be caught
print("Result:", result)


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   - 
Module: A Python file containing functions, classes, and variables that you can import and use in your scripts.
Package: A collection of related modules organized in a directory hierarchy.
Importing and Using Modules:
import math

# Use functions from the math module
area_of_circle = math.pi * (radius**2)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    - 
Reading from a file: Use the open() function with mode "r" (read).
Writing to a file: Use the open() function with mode "w" (write) or "a" (append).
Reading a File:
with open("myfile.txt", "r") as file:
    content = file.read()
    print("Content of the file:\n", content)

Writing a List to a File:
my_list = ["apple", "banana", "cherry"]
with open("fruits.txt", "w") as file:
    for item in my_list:
        file.write(item + "\n")  # Write each item with a newline

print("List written to the file")

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


