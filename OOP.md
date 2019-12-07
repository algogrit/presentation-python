## Classes in Python

- Classes are extremely important in programming.
- We have already learnt types such as numbers , strings and booleans.
- We have also learnt about lists and dictionaries.
- We use classes to define new types to model new concepts. eg : Shopping Cart

To define a class :

```python
class Point    # class called point is defined.
```
---
#### Class Objects and Instances

- A class name uses the Pascal Naming convention.
- That is the name of the class starts with a capital letter.
- If the class has multiple words then each word starts with a capital letter.
- First a class is defined.
- We add a colon to define a block.

---

- Under the class Point we can create operations / methods.
- As soon as we open parenthesis, Pycharm automatically adds self.
- Self is a special keyword.
- A class defines the blueprint or the  template for creating objects and the objects are the actual instances based on that blueprint.

---

#### Structure of a Python Class



```python
class Point:   # Colon is used to define a block. In this block we can define all the functions or methods that belong to that class.
    def move (self):   # Operations
        print("move")
    def draw (self):   # Operations
        print("draw")


point1 = Point() # Class object could be used to access different attributes. point1 is an instance.
point1.x = 10   #Attributes that can be set anywhere in the program
point1.y = 20
print(point1.x)
point1.draw()

point2 = Point()
point2.x = 1
print(point2.x)
```
---

#### The SELF Syntax

- By using the self keyword we can access the attributes and methods of a class in Python.
- It binds the attributes with the given arguments.
- self is parameter in function and user can use another name in place of it.
- It is advisable to use self because it increases the readability of code.
- Whenever an object calls its method , the object itself is passed as the first argument.
- The first argument of the function in class must be the object itself.


---

#### Inheritance

- Instead of starting from a scratch, you can create a class by deriving it from a pre-existing class by listing the parent class in parentheses after the new class name.

- The child class inherits the attributes of its parent class, and you can use those attributes as if they were defined in the child class.

- A child class can also override data members and methods from the parent.

Syntax
- Derived classes are declared much like their parent class; however, a list of base classes to inherit from is given after the class name −

```python
class SubClassName (ParentClass1[, ParentClass2, ...]):
   'Optional class documentation string'
   class_suite
```
---
