# PYTHON

## What is Python ?

- Python is a high level, case sensitive programming language designed to be easy to read and simple to implement.
- It is open source which means it is free to use even for commercial applications.

## Used in

- Building web applications.
- Building Desktop applications.
- Machine learning.
- Artificial intelligence.

---

## Downloading Python

- Go to Python.org
- Click on downloads where we can see the latest version of Python.
- Download Python. Check the downloads folder.
- Double click Python Installer.
- Check box 'Add Python 3.7 to PATH'.
- Python would be installed.

---

### Python Code editor

- Code editor to write code just like word to write documents
- Python has many code editors. One of the editors is PyCharm.
- PyCharm is a popular code editor for writing code.
- The Python Integrated development environment.

---

### Python Interpreter

- Converts python code into to way the machine can understand.
- Knows how to execute Python code.
- Python Interpreter runs the code line by line from the top.

### What are legacy systems?

- No longer maintained or supported.

---

### Creating a Python Program

- Right click on the new project created and create a new file.
- Click New - Python file
- All python files have an extension of .py

---

## Python Syntax Review

### Printing a statement

- `print("This is my first Python program")`
- Anything in between quotes denotes a string.
- Click Run

- `print ('*' * 10)`
- The string will be displayed 10 times. This is an expression.

---

Now try these commands :

### Defining Variables

```python
price = 10                  # int
rating = 4.8                # float
Name = 'Gaurav'             # str
boolean_variable = False    # bool
print(price)
```

Here price is a variable. This is how you define variables.

---

Question 1:

```python
price = 10
price = 20
print(price)
```

- What would you think the output will be ?

---

Question 2:

Write a program for a school for enrolling a student named Mark. He is 10 years old and is a new student. Define three variables for his name, age and another variable to tell if this is a new or existing student.

---

## Solution

- Ans 1: 20

- Ans 2:

```python
studentname = 'Mark'
studentage = 10
is_new = True
```

# Datatypes Overview

list , dict , tuple , set , string


## Strings

- We can define strings using single (' ') or double (" ") quotes.
- To define a multi-line string, we surround our string with triple quotes (""").
- We can get individual characters in a string using square brackets.

---

Now try these commands :

course = 'Python for Beginners'

```python
course[0]  # Returns the first Character
course[1]  # Returns the second Character
course[-1]  # Returns the first character from the end
course[-2]  # Returns the second character from the end
course[1:5]  # This expression returns all the characters starting from index position of 1 to 5 (but excluding 5)
len()       #Count the number of characters in a string. This is a general purpose function built into python.
```

---

We also have specific functions for strings which we refer to as methods.

``` python
course.upper()   # Converts a string into upper case
course.lower()   # Converts a string into lower case
course.title()   # To capitalize the first letter of every word.
course.find()    # Returns the index of a character or a sequence of characters.
course.replace()  # Replacing characters and words in a string
'...' in course  # Characters in a string
```

---

## Lists
```python

numbers = [1, 2, 3, 4, 5]
numbers[0]    # Returns the first item
numbers[1]    # Returns the second item
numbers[-1]   # Returns the first item from the last
numbers[-2]   # Returns the second item from the last
numbers.append(6) # Adds 6 to the end
numbers.insert(0,6)  # Replaces 6 at index position of 0
numbers.remove(6)  # Removes 6
numbers.pop()  # Removes the last item
numbers.clear()  # Removes all the items
numbers.index(8) # Returns the index of first occurrence of 8
numbers.sort()  # sorts the List
numbers.reverse() # reverses the List
numbers.copy() # Returns a copy of the List
```
---
## Dictionaries

We use dictionaries to store key/value pairs.

```python
customer = {
  "name" : "Gaurav Agarwal",
  "age": 30,
  "is_verified": True
}
```
We can use strings or numbers to define keys. They should be unique. We can use any types for the values.

```python
customer["name"]   # returns "Gaurav Agarwal"
 ```

---
##  Tuples

- They are like read only lists.
- We use them to store a list of items.
- Once we define a tuple we cannot add or remove items or change the existing items.

```python
coordinates = (1,2,3)
```

We can unpack a list or a tuple into separate variables.

```python
x,y,z = coordinates
```
---

















```
