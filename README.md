[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15316695&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
Python is a high-level, interpreted programming language. 
Key Features of Python
Simple and Readable Syntax: Python's syntax is clean and easy to understand, making it an excellent choice for beginners and enabling developers to write clear and maintainable code.

Interpreted Language: Python is an interpreted language, meaning that it executes code line by line, which makes debugging easier and accelerates the development process.

Dynamic Typing: Python uses dynamic typing, allowing variables to change type, which provides flexibility in coding and reduces the amount of boilerplate code.

Extensive Standard Library: Python comes with a comprehensive standard library that includes modules and packages for various tasks such as file I/O, system calls, and web development, which helps to minimize the need for external libraries.

Cross-Platform Compatibility: Python is cross-platform and can run on various operating systems, including Windows, macOS, and Linux, which allows developers to write code that is portable and adaptable.

Support for Multiple Programming Paradigms: Python supports various programming paradigms, including procedural, object-oriented, and functional programming, giving developers the flexibility to choose the best approach for their projects.

Use Cases Where Python is Particularly Effective:
1.Web Development: Python is widely used in web development due to frameworks like Django and Flask, which provide robust and scalable solutions for building web applications.
2.Data Science and Machine Learning: Python is a favorite in the data science and machine learning communities because of its powerful libraries such as NumPy, pandas, scikit-learn, and TensorFlow.
3.Automation and Scripting: Python’s simplicity and versatility make it ideal for writing scripts to automate repetitive tasks, such as file manipulation, web scraping, and system administration.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   on the terminal of linux use 'sudo apt install python' to install python.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   print('Hello, World!'):
   Explanation of  Syntax Elements
Function Call:

print("Hello, World!")
print is a built-in Python function used to output text or other data to the console. Functions are reusable blocks of code that perform a specific task.
Parentheses:

print(...)
The parentheses () are used to pass arguments to the function. In this case, we pass the string "Hello, World!" to the print function.
String:

"Hello, World!"
A string is a sequence of characters enclosed in quotation marks. In Python, strings can be enclosed in either single ('...') or double ("...") quotation marks. Here, we use double quotation marks to define the string that we want to print.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   1.String-Sequences of characters enclosed in quotes. Example: "Hello, World!", 'Python'.
   2.integer-Whole numbers, positive or negative, without decimals. Example: 10, -5
   3.boolean- Represents one of two values: True or False.
   4.float- Numbers that have a decimal point.
   5.list-collections of items which can be of any type. Example: [1, 2, 3], ['a', 'b', 'c'].
   6.tuples-immutable collections of items. Example: (1, 2, 3), ('a', 'b', 'c').
   7.Dictionaries-collections of key-value pairs. Example: {'name': 'Alice', 'age': 25}.
   8.sets-Unordered collections of unique items. Example: {1, 2, 3}, {'a', 'b', 'c'}.

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   Conditional statements are used to execute different blocks of code based on certain conditions. 
age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
Loops are used to execute a block of code repeatedly. The two main types of loops in Python are for and while.
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   Functions in Python are blocks of reusable code designed to perform a specific task. They help to modularize the code, making it more organized, readable, and easier to maintain. 
def add_numbers(a, b):   
   return a + b
result = add_numbers(5, 3)
print(f"The sum is: {result}")

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   Lists:

Ordered: Lists maintain the order of elements. The elements are indexed based on their position starting from 0.
Mutable: The elements in a list can be changed, added, or removed.
Elements: Lists can contain any type of objects, such as integers, strings, other lists, etc.
Access: Elements are accessed by their index positions.
Dictionaries:

Unordered: Dictionaries do not maintain the order of elements. Each element is a key-value pair.
Mutable: The elements in a dictionary can be changed, added, or removed.
Key-Value Pairs: Each element is a pair consisting of a unique key and a corresponding value.
Access: Values are accessed by their keys, not by their position.

# Creating a list of numbers
numbers_list = [10, 20, 30, 40, 50]
# Creating a dictionary with some key-value pairs
person_dict = {
    'name': 'Alice',
    'age': 30,
    'city': 'New York'
}

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
Exception Handling in Python
Exception handling in Python is a mechanism for responding to the occurrence of exceptions—runtime errors that disrupt the normal flow of the program. Python provides the try, except, else, and finally blocks to handle these exceptions gracefully.

try block: This is the block of code where exceptions are monitored. If an exception occurs, the rest of the block is skipped and the exception is caught by the corresponding except block.
except block: This block is executed when an exception occurs in the try block. You can have multiple except blocks to handle different types of exceptions.
else block: This block is executed if no exceptions occur in the try block.
finally block: This block is executed no matter what—whether an exception occurred or not. It is typically used for cleanup actions.

def divide(a, b):
    try:
        result = a / b
    except ZeroDivisionError as e:
        print(f"Error: Cannot divide by zero. {e}")
    except TypeError as e:
        print(f"Error: Invalid input types. {e}")
    else:
        print(f"Result: {result}")
    finally:
        print("Execution completed.")

# Example usage
print("Example 1:")
divide(10, 2)  # Valid division

print("\nExample 2:")
divide(10, 0)  # Division by zero

print("\nExample 3:")
divide(10, 'a')  # Invalid input type

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   Module: A module is a single Python file that contains a collection of related functions, classes, or variables. By organizing code into modules, you can logically divide your code into manageable and reusable pieces. Modules help to avoid code redundancy and make code maintenance easier.

Package: A package is a collection of related modules bundled together within a directory hierarchy. It contains a special file named __init__.py (which can be empty) that indicates to Python that the directory should be treated as a package. Packages enable a hierarchical structuring of the module namespace.

Importing and Using a Module:
1.Importing the whole module:
import math
2.Importing specific functions or variables from a module:
from math import sqrt, pi
3.Importing a module with an alias:
import math as m

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    In Python, you can use built-in functions to read from and write to files. The open() function is used to open a file, which returns a file object. You can then use methods such as read(), readline(), readlines(), write(), and writelines() to manipulate the file contents.

    # Reading from a file
try:
    with open('example.txt', 'r') as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("The file does not exist.")
except Exception as e:
    print(f"An error occurred: {e}")

   # Writing to a file
lines = [
    "This is the first line.\n",
    "This is the second line.\n",
    "This is the third line.\n"
]

try:
    with open('output.txt', 'w') as file:
        file.writelines(lines)
    print("The lines were successfully written to the file.")
except Exception as e:
    print(f"An error occurred: {e}")

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


