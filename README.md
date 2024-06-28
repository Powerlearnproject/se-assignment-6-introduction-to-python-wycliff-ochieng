[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15340636&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a high-level, interpreted programming language known for its readability, simplicity, and versatility.
   It has features such as: easy to read and write
                            interpretaed language
                            wide variety of standard library
                            large community of developers
                            Python is particularly effective in web development, data analysis, scientific computing, and machine learning
   It is widely used in web development,data analysis and visualization,Artificial intelligence and automation,webscraping,data science and machine learning

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Download the Installer:

Visit the official Python website.
Download the installer for your operating system (Windows, macOS, or Linux).
Run the Installer:

On Windows, run the .exe file and follow the installation wizard. Ensure you check the box to add Python to your PATH.
On macOS, run the .pkg file and follow the prompts.
On Linux, use the package manager (e.g., sudo apt install python3 for Debian-based systems).
Verify the Installation:

Open a terminal or command prompt.
Type python --version or python3 --version and press Enter. You should see the installed Python version.
Set Up a Virtual Environment:

Install virtualenv if necessary: pip install virtualenv.
Create a virtual environment: python -m venv myenv.
Activate the virtual environment:
Windows: myenv\Scripts\activate
(REFERENCES python.org)

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   print("Hello world")
   print() is a function that prints the string "Hello world" to the console.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

int: Integer numbers (e.g., 1, 42)
float: Floating-point numbers (e.g. 5.7,3.64)
str: Strings (e.g., "name")
bool: Boolean values (e.g., True, False)
list: Ordered, mutable collections (e.g., [4, 5, 6])
dict: Unordered, mutable collections of key-value pairs (e.g., {"name": "John", "age": 37})

 Creating variables
age = 30
name = "Mark"
weight = 5.9
student = False

print(f"Name: {name}, Age: {age}, Height: {height}, Student: {student}")


#functions
def area(a, b):
    return a * b

result = area(3, 5)
print(result)  



While loop
count = 0
while count < 5:
    print(count)
    count += 1




5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

 conditionals- are used to execute a block of code only if a certain condition is met. The most common conditional statements are if, elif, and else. 

weight = 65
if age >=65:
    print("You are overweight.Kindly exercise")
else:
    print("You have healthy body weight.")

For loop
for x in range(10):
    print(x)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions are reusable blocks of code that perform a specific task.
They are useful because
Reusability: Functions allow you to write a piece of code once and reuse it multiple times.
Modularity: Functions help in breaking down complex problems into smaller, manageable pieces.
Readability: Functions can make code more readable and easier to understand by providing meaningful names for blocks of code.

#functions
def area(a, b):
    return a * b

result = area(3, 5)
print(result) 

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

List are ordered while dictionary are unordered
Lists are mutable while dictionary are immutable
Lists are indexed while dictionary are not indexed

my_list = [4, 6, 7, 8, 2]
print(my_list)

my_context = {"age":34, "school":KU, "course":software technology}
print(my_context)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python is a mechanism to handle runtime errors, allowing a program to continue execution (or fail gracefully) when an error occurs

   def divide(a, b):
    try:
        result = a / b
    except ZeroDivisionError as e:
        print("Error: Cannot divide by zero.")
        return None
    except TypeError as e:
        print("Error: Invalid input types. Please provide numbers.")
        return None
    else:
        print("Division successful.")
        return result
    finally:
        print("Execution of the divide function is complete.")

# Example usage
print(divide(10, 2))   # Output: Division successful. 5.0 Execution of the divide function is complete.
print(divide(10, 0))   # Output: Error: Cannot divide by zero. None Execution of the divide function is complete.
print(divide(10, 'a')) # Output: Error: Invalid input types. Please provide numbers. None Execution of the divide function is complete.


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

A module is a single file (or files) that contains Python code, such as functions, classes, or variables.
It allows you to organize your code into smaller, manageable parts.A package is a way of organizing related modules into a directory hierarchy.

To use a module in your script, you need to import it using the import statement.Example

import math

print(math.pi)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from a File:

Use the open function with mode 'r' to open the file in read mode.
Use file.read() to read the content of the file.
Use a context manager (with statement) to ensure the file is closed after reading.

Writing to a File:
Use the open function with mode 'w' to open the file in write mode.
Use file.writelines() to write a list of strings to the file.
Use a context manager (with statement) to ensure the file is closed after writing.

Reading from a file
with open('word.txt', 'r') as file:
    paragraph = file.read()

print(paragraph)

Writing to a file
lines = [
    "First line of the file.\n",
    "Second line of the file.\n",
    "Third line of the file.\n"
]

with open('output.txt', 'w') as file:
    file.writelines(lines)



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


