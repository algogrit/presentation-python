# Advanced Data types and Functional Programming

## Datatypes:

### Namedtuple in Python

- Python supports a type of container like dictionaries called “namedtuples()” present in module, “collection“.
- Like dictionaries they contain keys that are hashed to a particular value.
- But on contrary, it supports both access from key value and iteration, the functionality that dictionaries lack.

---
Operations on namedtuple() :

Access Operations
1. Access by index : The attribute values of namedtuple() are ordered and
can be accessed using the index number unlike dictionaries which are not accessible by index.

2. Access by keyname : Access by keyname is also allowed as in dictionaries.

3. using getattr() :- This is yet another way to access the value by giving namedtuple and key value as its argument.
---

# Python code to demonstrate namedtuple() and
# Access by name, index and getattr()

# importing "collections" for namedtuple()
import collections

# Declaring namedtuple()
Student = collections.namedtuple('Student',['name','age','DOB'])

# Adding values
S = Student('Nandini','19','2541997')

# Access using index
print ("The Student age using index is : ",end ="")
print (S[1])

# Access using name
print ("The Student name using keyname is : ",end ="")
print (S.name)

# Access using getattr()
print ("The Student DOB using getattr() is : ",end ="")
print (getattr(S,'DOB'))

---

```python

Output :

The Student age using index is : 19
The Student name using keyname is : Nandini
The Student DOB using getattr() is : 2541997

```
---

### defaultdict

A defaultdict works exactly like a normal dict, but it is initialized with a function (“default factory”) that takes no arguments and provides the default value for a nonexistent key.

A defaultdict will never raise a KeyError. Any key that does not exist gets the value returned by the default factory.

```python

>>> from collections import defaultdict
>>> ice_cream = defaultdict(lambda: 'Vanilla')
>>>
>>> ice_cream = defaultdict(lambda: 'Vanilla')
>>> ice_cream['Sarah'] = 'Chunky Monkey'
>>> ice_cream['Abdul'] = 'Butter Pecan'
>>> print ice_cream['Sarah']
Chunky Monkey
>>> print ice_cream['Joe']
Vanilla
>>>

```

Be sure to pass the function object to defaultdict(). Do not call the function, i.e. defaultdict(func), not defaultdict(func()).

### Ordereddict

- An OrderedDict is a dictionary subclass that remembers the order that keys were first inserted.
 The only difference between dict() and OrderedDict() is that:
- OrderedDict preserves the order in which the keys are inserted. A regular dict doesn’t track the insertion order, and iterating it gives the values in an arbitrary order.
- By contrast, the order the items are inserted is remembered by OrderedDict.


# A Python program to demonstrate working of OrderedDict
from collections import OrderedDict

print("This is a Dict:\n")
d = {}
d['a'] = 1
d['b'] = 2
d['c'] = 3
d['d'] = 4

for key, value in d.items():
    print(key, value)

print("\nThis is an Ordered Dict:\n")
od = OrderedDict()
od['a'] = 1
od['b'] = 2
od['c'] = 3
od['d'] = 4

for key, value in od.items():
    print(key, value)

Output:

This is a Dict:
('a', 1)
('c', 3)
('b', 2)
('d', 4)

This is an Ordered Dict:
('a', 1)
('b', 2)
('c', 3)
('d', 4)


Deque


Deque can be implemented in python using the module “collections“. Deque is preferred over list in the cases where we need quicker append and pop operations from both the ends of container, as deque provides an O(1) time complexity for append and pop operations as compared to list which provides O(n) time complexity.

Operations on deque :

1. append() :- This function is used to insert the value in its argument to the right end of deque.

2. appendleft() :- This function is used to insert the value in its argument to the left end of deque.

3. pop() :- This function is used to delete an argument from the right end of deque.

4. popleft() :- This function is used to delete an argument from the left end of deque.




# Python code to demonstrate working of
# append(), appendleft(), pop(), and popleft()

# importing "collections" for deque operations
import collections

# initializing deque
de = collections.deque([1,2,3])

# using append() to insert element at right end
# inserts 4 at the end of deque
de.append(4)

# printing modified deque
print ("The deque after appending at right is : ")
print (de)

# using appendleft() to insert element at right end
# inserts 6 at the beginning of deque
de.appendleft(6)

# printing modified deque
print ("The deque after appending at left is : ")
print (de)

# using pop() to delete element from right end
# deletes 4 from the right end of deque
de.pop()

# printing modified deque
print ("The deque after deleting from right is : ")
print (de)

# using popleft() to delete element from left end
# deletes 6 from the left end of deque
de.popleft()

# printing modified deque
print ("The deque after deleting from left is : ")
print (de)
Output:

The deque after appending at right is :
deque([1, 2, 3, 4])
The deque after appending at left is :
deque([6, 1, 2, 3, 4])
The deque after deleting from right is :
deque([6, 1, 2, 3])
The deque after deleting from left is :
deque([1, 2, 3])
