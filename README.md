# Programming Roadmap Based on Python Syntax

## Objective

This roadmap is designed for beginners who want to learn **programming concepts using Python syntax**.

The goal is not only to memorize Python commands, but to understand how programming works in general:

* How to think logically
* How to solve problems step by step
* How to write clean code
* How to build small programs
* How to move from beginner level to backend/API development
* How to prepare for real software engineering projects

Python is a good first language because its syntax is simple, readable, and close to human language.

---

# Table of Contents

1. [Programming Fundamentals](#1-programming-fundamentals)
2. [Python Setup](#2-python-setup)
3. [Variables and Data Types](#3-variables-and-data-types)
4. [Input and Output](#4-input-and-output)
5. [Operators](#5-operators)
6. [Conditions and Decision Making](#6-conditions-and-decision-making)
7. [Loops](#7-loops)
8. [Strings](#8-strings)
9. [Lists](#9-lists)
10. [Tuples](#10-tuples)
11. [Sets](#11-sets)
12. [Dictionaries](#12-dictionaries)
13. [Functions](#13-functions)
14. [Error Handling](#14-error-handling)
15. [Files](#15-files)
16. [Modules and Packages](#16-modules-and-packages)
17. [Object-Oriented Programming](#17-object-oriented-programming)
18. [Working with Dates and Time](#18-working-with-dates-and-time)
19. [JSON and CSV](#19-json-and-csv)
20. [APIs and HTTP Requests](#20-apis-and-http-requests)
21. [Databases](#21-databases)
22. [Testing](#22-testing)
23. [Git and GitHub](#23-git-and-github)
24. [Intermediate Python](#24-intermediate-python)
25. [Web Development with Flask and FastAPI](#25-web-development-with-flask-and-fastapi)
26. [Automation and Scripting](#26-automation-and-scripting)
27. [Data Processing](#27-data-processing)
28. [Backend Engineering Basics](#28-backend-engineering-basics)
29. [Deployment Basics](#29-deployment-basics)
30. [Final Projects](#30-final-projects)
31. [Suggested Study Plan](#31-suggested-study-plan)

---

# 1. Programming Fundamentals

## Goal

Before learning Python deeply, understand what programming is.

Programming means giving instructions to a computer to solve a problem.

A program usually contains:

* Data
* Logic
* Conditions
* Repetition
* Functions
* Input
* Output

## Concepts to Understand

### What is a Program?

A program is a set of instructions.

Example:

```python
print("Hello, World!")
```

This program tells the computer to display text.

---

### What is Syntax?

Syntax means the rules of writing code.

Example of correct Python syntax:

```python
name = "Ali"
print(name)
```

Example of wrong syntax:

```python
name = "Ali
print(name)
```

The second example is wrong because the string is not closed.

---

### What is a Bug?

A bug is an error in the program.

Types of bugs:

* Syntax error
* Logic error
* Runtime error

Example of syntax error:

```python
print("Hello"
```

Example of logic error:

```python
price = 100
discount = 10

final_price = price + discount
print(final_price)
```

The program runs, but the logic is wrong. Discount should be subtracted, not added.

Correct version:

```python
final_price = price - discount
print(final_price)
```

---

# 2. Python Setup

## Goal

Install Python and learn how to run Python programs.

## Tools Needed

Install:

* Python
* VS Code
* Python extension for VS Code
* Git
* Terminal or Command Prompt

## Check Python Version

```bash
python --version
```

or:

```bash
python3 --version
```

## Run Python File

Create a file:

```text
main.py
```

Write:

```python
print("Hello Python")
```

Run:

```bash
python main.py
```

## Practice

Create these files:

```text
hello.py
calculator.py
profile.py
```

---

# 3. Variables and Data Types

## Goal

Learn how to store data in memory.

A variable is a name that stores a value.

```python
name = "Ali"
age = 20
salary = 5000.50
is_active = True
```

## Common Data Types

| Type    | Example           | Description          |
| ------- | ----------------- | -------------------- |
| `str`   | `"Ali"`           | Text                 |
| `int`   | `20`              | Whole number         |
| `float` | `99.5`            | Decimal number       |
| `bool`  | `True`            | True or false        |
| `list`  | `[1, 2, 3]`       | Collection of values |
| `dict`  | `{"name": "Ali"}` | Key-value data       |

## Example

```python
student_name = "Mona"
student_age = 18
student_grade = 95.5
passed = True

print(student_name)
print(student_age)
print(student_grade)
print(passed)
```

## Naming Rules

Good variable names:

```python
user_name = "Ali"
total_price = 500
is_paid = False
```

Bad variable names:

```python
x = "Ali"
tp = 500
p = False
```

Use meaningful names.

## Practice

Create variables for:

* Customer name
* Customer age
* Product name
* Product price
* Quantity
* Is product available?

Example:

```python
customer_name = "Ahmed"
product_name = "Laptop"
price = 15000
quantity = 2
is_available = True
```

---

# 4. Input and Output

## Goal

Learn how to receive input from the user and display output.

## Output

```python
print("Welcome to Python")
```

## Input

```python
name = input("Enter your name: ")
print("Hello", name)
```

## Important Note

Input is always received as text.

Example:

```python
age = input("Enter your age: ")
print(type(age))
```

Even if the user enters `20`, Python treats it as text.

## Convert Input

```python
age = int(input("Enter your age: "))
print(age + 5)
```

## Example: Simple Age Program

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))

print("Hello", name)
print("After 5 years, your age will be", age + 5)
```

## Practice

Build:

1. Name greeting program
2. Age after 10 years
3. Simple calculator
4. Product total price calculator

Example:

```python
price = float(input("Enter product price: "))
quantity = int(input("Enter quantity: "))

total = price * quantity

print("Total price:", total)
```

---

# 5. Operators

## Goal

Learn how to perform calculations and comparisons.

## Arithmetic Operators

| Operator | Meaning        | Example  |
| -------- | -------------- | -------- |
| `+`      | Addition       | `5 + 3`  |
| `-`      | Subtraction    | `5 - 3`  |
| `*`      | Multiplication | `5 * 3`  |
| `/`      | Division       | `5 / 3`  |
| `//`     | Floor division | `5 // 3` |
| `%`      | Modulus        | `5 % 3`  |
| `**`     | Power          | `5 ** 3` |

## Example

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

## Comparison Operators

| Operator | Meaning               |
| -------- | --------------------- |
| `==`     | Equal                 |
| `!=`     | Not equal             |
| `>`      | Greater than          |
| `<`      | Less than             |
| `>=`     | Greater than or equal |
| `<=`     | Less than or equal    |

Example:

```python
age = 20

print(age >= 18)
print(age < 18)
```

## Logical Operators

| Operator | Meaning                             |
| -------- | ----------------------------------- |
| `and`    | Both conditions must be true        |
| `or`     | At least one condition must be true |
| `not`    | Reverse result                      |

Example:

```python
age = 25
has_id = True

can_enter = age >= 18 and has_id == True

print(can_enter)
```

## Practice

Build:

* Tax calculator
* Discount calculator
* Loan eligibility checker
* Even or odd checker

---

# 6. Conditions and Decision Making

## Goal

Make programs choose different actions based on conditions.

## Basic If Statement

```python
age = 18

if age >= 18:
    print("Adult")
```

## If Else

```python
age = 16

if age >= 18:
    print("Adult")
else:
    print("Child")
```

## If Elif Else

```python
grade = 85

if grade >= 90:
    print("Excellent")
elif grade >= 75:
    print("Very Good")
elif grade >= 60:
    print("Good")
else:
    print("Failed")
```

## Nested Conditions

```python
username = "admin"
password = "1234"

if username == "admin":
    if password == "1234":
        print("Login successful")
    else:
        print("Wrong password")
else:
    print("Unknown user")
```

## Practice Projects

### 1. Student Grade System

Input:

* Student name
* Degree

Output:

* Excellent
* Very good
* Good
* Failed

### 2. Login System

Input:

* Username
* Password

Output:

* Login success
* Wrong username
* Wrong password

### 3. Discount Calculator

Rules:

* If total >= 1000, discount = 10%
* If total >= 500, discount = 5%
* Otherwise, no discount

---

# 7. Loops

## Goal

Repeat instructions multiple times.

Python has two main loops:

* `for`
* `while`

---

## For Loop

Use `for` when you know how many times to repeat.

```python
for i in range(5):
    print(i)
```

Output:

```text
0
1
2
3
4
```

## Range

```python
for i in range(1, 6):
    print(i)
```

Output:

```text
1
2
3
4
5
```

## While Loop

Use `while` when repetition depends on a condition.

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

## Break

Stop the loop.

```python
for i in range(1, 10):
    if i == 5:
        break
    print(i)
```

## Continue

Skip current iteration.

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

## Practice Projects

### 1. Multiplication Table

```python
number = int(input("Enter number: "))

for i in range(1, 13):
    print(number, "x", i, "=", number * i)
```

### 2. Sum Numbers from 1 to N

```python
n = int(input("Enter number: "))
total = 0

for i in range(1, n + 1):
    total += i

print("Total:", total)
```

### 3. Password Retry System

```python
correct_password = "1234"
attempts = 3

while attempts > 0:
    password = input("Enter password: ")

    if password == correct_password:
        print("Login successful")
        break
    else:
        attempts -= 1
        print("Wrong password. Attempts left:", attempts)

if attempts == 0:
    print("Account locked")
```

---

# 8. Strings

## Goal

Learn how to work with text.

## Create String

```python
name = "Ahmed"
message = 'Hello'
```

## String Concatenation

```python
first_name = "Ali"
last_name = "Hassan"

full_name = first_name + " " + last_name

print(full_name)
```

## F-Strings

Recommended way:

```python
name = "Ali"
age = 20

print(f"My name is {name} and I am {age} years old")
```

## Common String Methods

```python
text = " hello python "

print(text.upper())
print(text.lower())
print(text.strip())
print(text.replace("python", "world"))
print(text.title())
```

## String Indexing

```python
name = "Python"

print(name[0])
print(name[1])
print(name[-1])
```

## String Slicing

```python
name = "Python"

print(name[0:3])
print(name[2:])
print(name[:4])
```

## Practice

Build:

* Username formatter
* Email validator
* Search word in sentence
* Full name generator

Example:

```python
email = input("Enter email: ")

if "@" in email and "." in email:
    print("Valid email")
else:
    print("Invalid email")
```

---

# 9. Lists

## Goal

Store multiple values in one variable.

## Create List

```python
students = ["Ali", "Mona", "Sara"]
```

## Access Items

```python
print(students[0])
print(students[1])
```

## Add Item

```python
students.append("Omar")
```

## Remove Item

```python
students.remove("Ali")
```

## Loop Over List

```python
for student in students:
    print(student)
```

## List Length

```python
print(len(students))
```

## List of Numbers

```python
numbers = [10, 20, 30, 40]

total = 0

for number in numbers:
    total += number

print(total)
```

## Practice Projects

### 1. Student Names List

Features:

* Add student
* Remove student
* Show all students

### 2. Shopping Cart

Features:

* Add product
* Remove product
* Show cart
* Count items

### 3. Marks Average

```python
marks = [90, 80, 70, 100]

total = sum(marks)
average = total / len(marks)

print("Average:", average)
```

---

# 10. Tuples

## Goal

Store fixed data that should not change.

## Create Tuple

```python
point = (10, 20)
```

## Example

```python
days = ("Saturday", "Sunday", "Monday")

print(days[0])
```

## Difference Between List and Tuple

| List                  | Tuple               |
| --------------------- | ------------------- |
| Can change            | Cannot change       |
| Uses `[]`             | Uses `()`           |
| Good for dynamic data | Good for fixed data |

## Practice

Use tuples for:

* Days of week
* Coordinates
* Fixed configuration values

---

# 11. Sets

## Goal

Store unique values.

## Create Set

```python
numbers = {1, 2, 3, 3, 4}
print(numbers)
```

Output:

```text
{1, 2, 3, 4}
```

## Add Item

```python
numbers.add(5)
```

## Remove Item

```python
numbers.remove(2)
```

## Practice

Use sets for:

* Unique student names
* Unique product codes
* Unique tags

Example:

```python
emails = ["a@test.com", "b@test.com", "a@test.com"]
unique_emails = set(emails)

print(unique_emails)
```

---

# 12. Dictionaries

## Goal

Store key-value data.

## Create Dictionary

```python
user = {
    "name": "Ali",
    "age": 25,
    "city": "Cairo"
}
```

## Access Value

```python
print(user["name"])
```

## Safer Access

```python
print(user.get("email", "No email found"))
```

## Add or Update Value

```python
user["email"] = "ali@example.com"
user["age"] = 26
```

## Loop Over Dictionary

```python
for key, value in user.items():
    print(key, value)
```

## Practice Projects

### 1. Contact Book

```python
contacts = {
    "Ali": "01000000000",
    "Mona": "01111111111"
}
```

Features:

* Add contact
* Search contact
* Delete contact
* Show all contacts

### 2. Product Object

```python
product = {
    "id": 1,
    "name": "Laptop",
    "price": 15000,
    "stock": 10
}
```

---

# 13. Functions

## Goal

Reuse code and organize your program.

## Basic Function

```python
def say_hello():
    print("Hello")
```

Call the function:

```python
say_hello()
```

## Function with Parameters

```python
def greet(name):
    print(f"Hello {name}")

greet("Ali")
```

## Function with Return Value

```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)
```

## Default Parameters

```python
def greet(name="Guest"):
    print(f"Hello {name}")

greet()
greet("Mona")
```

## Practice

Create functions for:

* Add two numbers
* Calculate tax
* Calculate discount
* Validate email
* Convert temperature
* Calculate average

Example:

```python
def calculate_discount(total):
    if total >= 1000:
        return total * 0.10
    elif total >= 500:
        return total * 0.05
    else:
        return 0


total = 1200
discount = calculate_discount(total)
final_total = total - discount

print(final_total)
```

---

# 14. Error Handling

## Goal

Prevent the program from crashing when errors happen.

## Try Except

```python
try:
    number = int(input("Enter number: "))
    print(10 / number)
except:
    print("Something went wrong")
```

## Specific Exceptions

```python
try:
    number = int(input("Enter number: "))
    print(10 / number)
except ValueError:
    print("Invalid number")
except ZeroDivisionError:
    print("Cannot divide by zero")
```

## Finally

```python
try:
    file = open("data.txt", "r")
    print(file.read())
except FileNotFoundError:
    print("File not found")
finally:
    print("Program finished")
```

## Practice

Build:

* Safe calculator
* Safe login system
* File reader
* User input validator

---

# 15. Files

## Goal

Read and write data using files.

## Write File

```python
with open("notes.txt", "w") as file:
    file.write("Hello Python")
```

## Read File

```python
with open("notes.txt", "r") as file:
    content = file.read()
    print(content)
```

## Append File

```python
with open("notes.txt", "a") as file:
    file.write("\nNew note")
```

## Read Lines

```python
with open("notes.txt", "r") as file:
    lines = file.readlines()

for line in lines:
    print(line.strip())
```

## Practice Projects

### 1. Notes App

Features:

* Add note
* Show notes
* Delete notes file

### 2. Simple Logger

Write logs to file:

```python
with open("app.log", "a") as file:
    file.write("User logged in\n")
```

---

# 16. Modules and Packages

## Goal

Organize code and reuse existing libraries.

## Import Built-in Module

```python
import math

print(math.sqrt(16))
```

## Import Specific Function

```python
from math import sqrt

print(sqrt(25))
```

## Create Your Own Module

Create file:

```text
calculator.py
```

```python
def add(a, b):
    return a + b
```

Create file:

```text
main.py
```

```python
from calculator import add

print(add(5, 3))
```

## Install Package

```bash
pip install requests
```

## Useful Modules

| Module     | Usage                       |
| ---------- | --------------------------- |
| `math`     | Math operations             |
| `random`   | Random numbers              |
| `datetime` | Dates and time              |
| `os`       | Operating system operations |
| `json`     | JSON files                  |
| `csv`      | CSV files                   |
| `requests` | HTTP requests               |

---

# 17. Object-Oriented Programming

## Goal

Model real-world things using classes and objects.

## Class

A class is a blueprint.

```python
class Student:
    pass
```

## Object

An object is an instance from a class.

```python
student1 = Student()
```

## Constructor

```python
class Student:
    def __init__(self, name, grade):
        self.name = name
        self.grade = grade
```

## Method

```python
class Student:
    def __init__(self, name, grade):
        self.name = name
        self.grade = grade

    def show_info(self):
        print(f"Name: {self.name}, Grade: {self.grade}")


student = Student("Ali", 90)
student.show_info()
```

## Inheritance

```python
class User:
    def __init__(self, name):
        self.name = name

    def login(self):
        print(f"{self.name} logged in")


class Admin(User):
    def delete_user(self):
        print("User deleted")


admin = Admin("Hassan")
admin.login()
admin.delete_user()
```

## Practice Projects

Build classes for:

* Student
* Teacher
* Product
* Order
* Bank Account
* Book
* Library

Example:

```python
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount

    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
        else:
            print("Not enough balance")

    def show_balance(self):
        print(f"Balance: {self.balance}")


account = BankAccount("Ali", 1000)
account.deposit(500)
account.withdraw(300)
account.show_balance()
```

---

# 18. Working with Dates and Time

## Goal

Handle dates, times, and durations.

## Import Datetime

```python
from datetime import datetime
```

## Current Date and Time

```python
now = datetime.now()
print(now)
```

## Format Date

```python
print(now.strftime("%Y-%m-%d"))
print(now.strftime("%H:%M:%S"))
```

## Create Date

```python
from datetime import date

birth_date = date(2000, 5, 10)
print(birth_date)
```

## Practice

Build:

* Age calculator
* Days between two dates
* Task deadline checker
* Simple attendance timestamp system

---

# 19. JSON and CSV

## JSON

JSON is common in APIs and configuration files.

## Dictionary to JSON

```python
import json

user = {
    "name": "Ali",
    "age": 25
}

json_text = json.dumps(user)
print(json_text)
```

## Write JSON File

```python
import json

user = {
    "name": "Ali",
    "age": 25
}

with open("user.json", "w") as file:
    json.dump(user, file)
```

## Read JSON File

```python
import json

with open("user.json", "r") as file:
    user = json.load(file)

print(user["name"])
```

## CSV

CSV is useful for tables and Excel-like data.

## Write CSV

```python
import csv

with open("students.csv", "w", newline="") as file:
    writer = csv.writer(file)
    writer.writerow(["Name", "Grade"])
    writer.writerow(["Ali", 90])
    writer.writerow(["Mona", 85])
```

## Read CSV

```python
import csv

with open("students.csv", "r") as file:
    reader = csv.reader(file)

    for row in reader:
        print(row)
```

## Practice

Build:

* Save users to JSON
* Read products from CSV
* Export student grades to CSV
* Import contacts from CSV

---

# 20. APIs and HTTP Requests

## Goal

Learn how programs communicate with other systems.

## What is an API?

An API allows one program to talk to another program.

Examples:

* Weather API
* Payment API
* SMS API
* Google Maps API
* GitHub API

## HTTP Methods

| Method   | Usage               |
| -------- | ------------------- |
| `GET`    | Read data           |
| `POST`   | Create data         |
| `PUT`    | Update full data    |
| `PATCH`  | Update partial data |
| `DELETE` | Delete data         |

## Install Requests

```bash
pip install requests
```

## GET Request

```python
import requests

response = requests.get("https://api.github.com")
data = response.json()

print(data)
```

## POST Request

```python
import requests

payload = {
    "name": "Ali",
    "email": "ali@example.com"
}

response = requests.post("https://example.com/users", json=payload)

print(response.status_code)
```

## Practice

Build:

* GitHub profile reader
* Weather app
* Currency exchange app
* Public API browser

---

# 21. Databases

## Goal

Store data permanently in a structured way.

Start with SQLite, then move to PostgreSQL.

---

## SQLite Example

```python
import sqlite3

conn = sqlite3.connect("app.db")
cursor = conn.cursor()

cursor.execute("""
CREATE TABLE IF NOT EXISTS users (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT NOT NULL,
    email TEXT NOT NULL
)
""")

conn.commit()
conn.close()
```

## Insert Data

```python
import sqlite3

conn = sqlite3.connect("app.db")
cursor = conn.cursor()

cursor.execute(
    "INSERT INTO users (name, email) VALUES (?, ?)",
    ("Ali", "ali@example.com")
)

conn.commit()
conn.close()
```

## Read Data

```python
import sqlite3

conn = sqlite3.connect("app.db")
cursor = conn.cursor()

cursor.execute("SELECT * FROM users")
users = cursor.fetchall()

for user in users:
    print(user)

conn.close()
```

## Database Concepts

Learn:

* Table
* Row
* Column
* Primary key
* Foreign key
* Index
* CRUD
* Relationship
* Join

## Practice Projects

Build:

* Todo database
* Student database
* Products database
* Orders database
* Contact book with SQLite

---

# 22. Testing

## Goal

Make sure your code works correctly.

## Install Pytest

```bash
pip install pytest
```

## Simple Function

```python
def add(a, b):
    return a + b
```

## Test Function

Create file:

```text
test_calculator.py
```

```python
def test_add():
    assert add(2, 3) == 5
```

## Run Tests

```bash
pytest
```

## What to Test

Test:

* Functions
* Business rules
* Validation
* API endpoints
* Database logic

## Practice

Write tests for:

* Calculator
* Discount function
* Email validator
* Login checker
* Grade calculator

---

# 23. Git and GitHub

## Goal

Track code changes and share projects.

## Initialize Git

```bash
git init
```

## Add Files

```bash
git add .
```

## Commit

```bash
git commit -m "initial commit"
```

## Create Branch

```bash
git branch feature-login
```

## Switch Branch

```bash
git checkout feature-login
```

or:

```bash
git switch feature-login
```

## Push to GitHub

```bash
git remote add origin https://github.com/username/repository.git
git push -u origin main
```

## Learn

* Repository
* Commit
* Branch
* Merge
* Pull request
* Clone
* Push
* Pull
* `.gitignore`

---

# 24. Intermediate Python

## Goal

Write more professional Python code.

## List Comprehension

```python
numbers = [1, 2, 3, 4, 5]

squares = [number * number for number in numbers]

print(squares)
```

## Lambda

```python
add = lambda a, b: a + b

print(add(5, 3))
```

## Type Hints

```python
def greet(name: str) -> str:
    return f"Hello {name}"
```

## Decorators

```python
def log_function(func):
    def wrapper():
        print("Function started")
        func()
        print("Function finished")
    return wrapper


@log_function
def say_hello():
    print("Hello")


say_hello()
```

## Generators

```python
def count_numbers():
    for i in range(1, 6):
        yield i


for number in count_numbers():
    print(number)
```

## Context Managers

```python
with open("data.txt", "r") as file:
    content = file.read()
```

## Practice

Build:

* Custom logger decorator
* Data filter function
* File processor
* Report generator
* Simple validation library

---

# 25. Web Development with Flask and FastAPI

## Goal

Build web applications and APIs.

---

## Flask

Good for beginners.

Install:

```bash
pip install flask
```

Example:

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello Flask"

app.run(debug=True)
```

---

## FastAPI

Recommended for modern APIs.

Install:

```bash
pip install fastapi uvicorn
```

Example:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def home():
    return {"message": "Hello FastAPI"}
```

Run:

```bash
uvicorn main:app --reload
```

## FastAPI Path Parameter

```python
@app.get("/users/{user_id}")
def get_user(user_id: int):
    return {"user_id": user_id}
```

## FastAPI Request Body

```python
from pydantic import BaseModel


class UserCreate(BaseModel):
    name: str
    email: str


@app.post("/users")
def create_user(user: UserCreate):
    return user
```

## Practice APIs

Build:

* Todo API
* Student API
* Product API
* Authentication API
* Blog API
* Inventory API

---

# 26. Automation and Scripting

## Goal

Use Python to automate repeated tasks.

## Examples

Python can automate:

* Rename files
* Organize folders
* Read Excel files
* Generate reports
* Send emails
* Scrape websites
* Monitor logs

## File Organizer Example

```python
import os
import shutil

source_folder = "downloads"

for filename in os.listdir(source_folder):
    if filename.endswith(".pdf"):
        shutil.move(
            os.path.join(source_folder, filename),
            os.path.join(source_folder, "pdfs", filename)
        )
```

## Practice

Build:

* File organizer
* Backup script
* Log cleaner
* Excel report generator
* Image resize script

---

# 27. Data Processing

## Goal

Process, clean, and analyze data.

## Install Pandas

```bash
pip install pandas openpyxl
```

## Read CSV

```python
import pandas as pd

df = pd.read_csv("sales.csv")
print(df.head())
```

## Read Excel

```python
import pandas as pd

df = pd.read_excel("sales.xlsx")
print(df.head())
```

## Basic Analysis

```python
print(df.describe())
print(df["amount"].sum())
print(df["amount"].mean())
```

## Practice

Build:

* Sales report
* Student marks report
* Inventory report
* CSV cleaner
* Excel merger

---

# 28. Backend Engineering Basics

## Goal

Move from writing scripts to building real backend systems.

## Concepts to Learn

* HTTP APIs
* REST
* Authentication
* Authorization
* Database design
* Service layer
* Repository layer
* DTOs
* Validation
* Logging
* Configuration
* Error handling
* Background jobs
* Caching
* Docker

## Suggested Project Structure

```text
project/
├── app/
│   ├── api/
│   │   └── routes.py
│   ├── core/
│   │   └── config.py
│   ├── domain/
│   │   └── models.py
│   ├── services/
│   │   └── user_service.py
│   ├── repositories/
│   │   └── user_repository.py
│   └── main.py
├── tests/
├── requirements.txt
├── README.md
└── .env
```

## Backend Projects

Build:

* User management API
* Product catalog API
* Order management API
* Payment simulation API
* Notification service
* Reporting API

---

# 29. Deployment Basics

## Goal

Run your application outside your computer.

## Learn

* Linux basics
* Environment variables
* Docker
* Docker Compose
* Nginx
* Cloud hosting
* Logs
* Monitoring

## Dockerfile Example

```dockerfile
FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

CMD ["python", "main.py"]
```

## Docker Compose Example

```yaml
services:
  app:
    build: .
    ports:
      - "8000:8000"
```

## Deployment Platforms

Beginner-friendly:

* Render
* Railway
* Fly.io
* PythonAnywhere

More advanced:

* DigitalOcean
* AWS
* Azure
* Google Cloud
* Kubernetes

---

# 30. Final Projects

## Beginner Projects

| Project              | Concepts                    |
| -------------------- | --------------------------- |
| Calculator           | Input, operators, functions |
| Number guessing game | Conditions, loops           |
| Student grade system | Conditions                  |
| Multiplication table | Loops                       |
| Notes app            | Files                       |
| Contact book         | Dictionaries                |
| Password generator   | Random, strings             |
| Todo CLI             | Lists, files                |

---

## Intermediate Projects

| Project                   | Concepts         |
| ------------------------- | ---------------- |
| Todo API                  | FastAPI, CRUD    |
| Blog API                  | API, database    |
| Inventory system          | OOP, database    |
| Student management system | OOP, SQLite      |
| Weather app               | API requests     |
| Expense tracker           | Files, database  |
| Excel report generator    | Pandas, openpyxl |

---

## Advanced Projects

| Project                 | Concepts                     |
| ----------------------- | ---------------------------- |
| E-commerce backend      | Users, products, orders      |
| Mini ERP                | Inventory, sales, purchases  |
| Document management API | Uploads, metadata, search    |
| Workflow engine basics  | Steps, conditions, execution |
| Reporting system        | SQL, filters, exports        |
| AI document extractor   | OCR, API, JSON schema        |
| Authentication service  | JWT, users, roles            |

---

# 31. Suggested Study Plan

## Month 1: Python Basics

### Week 1

Learn:

* Python setup
* Variables
* Data types
* Input/output
* Operators

Practice:

* Calculator
* Age calculator
* Product total calculator

---

### Week 2

Learn:

* Conditions
* Logical operators
* Nested conditions

Practice:

* Login checker
* Grade system
* Discount calculator

---

### Week 3

Learn:

* For loops
* While loops
* Break
* Continue

Practice:

* Multiplication table
* Password retry system
* Number guessing game

---

### Week 4

Learn:

* Strings
* Lists
* Dictionaries

Practice:

* Contact book
* Shopping cart
* Student list manager

---

# Month 2: Core Programming

### Week 5

Learn:

* Functions
* Parameters
* Return values
* Scope

Practice:

* Calculator with functions
* Tax calculator
* Email validator

---

### Week 6

Learn:

* Error handling
* Files
* JSON

Practice:

* Notes app
* Save users to JSON
* Safe calculator

---

### Week 7

Learn:

* OOP basics
* Classes
* Objects
* Methods

Practice:

* Bank account class
* Student class
* Product class

---

### Week 8

Learn:

* Inheritance
* Modules
* Packages

Practice:

* Library system
* Inventory system
* Split code into modules

---

# Month 3: Real Applications

### Week 9

Learn:

* APIs
* HTTP
* Requests
* JSON responses

Practice:

* Weather app
* GitHub profile app
* Currency app

---

### Week 10

Learn:

* SQLite
* CRUD
* SQL basics

Practice:

* Todo database
* Student database
* Contact database

---

### Week 11

Learn:

* Flask or FastAPI
* API routes
* Request body
* Response JSON

Practice:

* Todo API
* Student API
* Product API

---

### Week 12

Learn:

* Testing
* Git
* Project structure

Practice:

* Add tests to previous projects
* Push projects to GitHub
* Write README files

---

# Recommended Learning Order

```text
Python Setup
→ Variables
→ Input/Output
→ Operators
→ Conditions
→ Loops
→ Strings
→ Lists
→ Dictionaries
→ Functions
→ Error Handling
→ Files
→ JSON/CSV
→ OOP
→ Modules
→ APIs
→ Databases
→ Testing
→ Git
→ FastAPI
→ Docker
→ Real Projects
```

---

# Daily Study Routine

## 1 Hour Per Day

| Time   | Activity          |
| ------ | ----------------- |
| 15 min | Read/watch lesson |
| 25 min | Write code        |
| 10 min | Fix errors        |
| 10 min | Write notes       |

## 2 Hours Per Day

| Time   | Activity          |
| ------ | ----------------- |
| 30 min | Learn new concept |
| 60 min | Practice coding   |
| 20 min | Refactor code     |
| 10 min | Push to GitHub    |

---

# Rules for Learning Programming

## Rule 1: Write Code Daily

Do not only watch tutorials.

You must write code.

## Rule 2: Build Small Projects

Every concept should have a small project.

Example:

* Conditions → grade system
* Loops → multiplication table
* Files → notes app
* OOP → bank account system
* API → weather app

## Rule 3: Read Error Messages

Errors are part of learning.

Do not fear them.

## Rule 4: Use GitHub

Save every project.

Your GitHub will become your portfolio.

## Rule 5: Explain Your Code

After writing code, explain it in simple English.

If you cannot explain it, you did not fully understand it.

---

# Minimum Portfolio After 3 Months

By the end of 3 months, you should have:

1. Calculator
2. Grade system
3. Number guessing game
4. Contact book
5. Notes app
6. Bank account OOP project
7. Weather API app
8. Todo SQLite app
9. Todo FastAPI app
10. One complete backend project

---

# Final Recommended Backend Project

## Project Name

Student Management API

## Features

* Create student
* Update student
* Delete student
* List students
* Search students
* Store students in database
* Validate input
* Handle errors
* Add tests
* Write README
* Deploy API

## Technologies

* Python
* FastAPI
* SQLite or PostgreSQL
* Pydantic
* Pytest
* GitHub
* Docker

## Example API Endpoints

| Method   | Endpoint         | Description       |
| -------- | ---------------- | ----------------- |
| `GET`    | `/students`      | List students     |
| `GET`    | `/students/{id}` | Get student by ID |
| `POST`   | `/students`      | Create student    |
| `PUT`    | `/students/{id}` | Update student    |
| `DELETE` | `/students/{id}` | Delete student    |

---

# Final Advice

Do not rush.

Programming is learned by practice, not memorization.

Start with simple Python syntax, then use every concept to build small real programs.

The best path is:

```text
Learn concept
→ Write small example
→ Build small project
→ Fix errors
→ Improve code
→ Push to GitHub
```

After this roadmap, you will be ready to continue into:

* Backend development
* Data engineering
* Automation
* AI scripting
* APIs
* Databases
* Full-stack development
