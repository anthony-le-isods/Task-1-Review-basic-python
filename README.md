# DATA TYPES <span style="color:red"></span>
### Example 1: Integers
x = 10
print(type(x))  # Output: <class 'int'>

### Example 2: Strings
name = "Emmy"
print(type(name))  # Output: <class 'str'>

### Example 3: Lists
numbers = [1, 2, 3, 4]
print(type(numbers))  # Output: <class 'list'>

### Example 4: Floats
pi = 3.14
print(type(pi))  # Output: <class 'float'>

### Example 5: Booleans
is_raining = True
print(type(is_raining))  # Output: <class 'bool'>

### Example 6: Tuples
coordinates = (10, 20)
print(type(coordinates))  # Output: <class 'tuple'>


# CONDITION AND LOOPING
### Example 1: if-else condition
age = 18
if age >= 18:
    print("You can vote!")
else:
    print("Sorry, you are not old enough to vote.")

### Example 2: for loop
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

### Example 3: while loop
count = 1
while count <= 5:
    print(count)
    count += 1

### Example 4: Nested if-else condition
age = 18
gender = "female"
if age >= 18:
    if gender == "male":
        print("You can vote!")
    else:
        print("You are eligible to vote.")
else:
    print("Sorry, you are not old enough to vote.")

### Example 5: while loop with else block
count = 1
while count <= 5:
    print(count)
    count += 1
else:
    print("Count is greater than 5.")

### Example 6: for loop with continue statement
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    if num % 2 == 0:
        continue
    print(num)

# CLASS: DOCUMENT 
### Example 1: Creating a Document class
class Document:
    def __init__(self, docs_id, category_id, brief, content, created_date, authors):
        self.docs_id = docs_id
        self.category_id = category_id
        self.brief = brief
        self.content = content
        self.created_date = created_date
        self.authors = authors

### Example 2: Creating a Document object
doc1 = Document(1, 2, "Brief for Document 1", "Content for Document 1", "2022-01-01", ["Emmy", "Emma"])

### Example 3: Accessing attributes of a Document object
print(doc1.brief)  # Output: "Brief for Document 1"

# DATA STRUCTURE
### Example 1: List of Document objects
docs_list = [doc1, doc2, doc3]

### Example 2: Tuple of Document objects
docs_tuple = (doc1, doc2, doc3)

### Example 3: Dictionary of Document objects
docs_dict = {doc1.docs_id: doc1, doc2.docs_id: doc2, doc3.docs_id: doc3}

# MODULE 
### Example 1: Using the os module
import os

### Check if a file exists
if os.path.exists("file.txt"):
    print("File exists.")
else:
    print("File does not exist.")

### Example 2: Using the sys module
import sys

### Get the command-line arguments
args = sys.argv
print(args)

### Example 3: Using the datetime module
import datetime

### Get the current date and time
now = datetime.datetime.now()
print(now)

# ECEPTIONAL HANDLING
### Example 1: Handling an exception with try-except block
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Cannot divide by zero.")

### Example 2: Raising an exception
age = -1
if age < 0:
    raise ValueError("Age cannot be negative.")

### Example 3: Handling multiple exceptions with try-except block
try:
    x = int(input("Enter a number: "))
    y = 1 / x
except ValueError:
    print("Invalid input.")
except ZeroDivisionError:
    print("Cannot divide by zero.")
