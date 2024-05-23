# Coursera - Python Notes

- 'del' keyword can delete variables in Python

#### Typecasting 
The process of converting one data type to another

**Implicit conversion** - if data types are compatible, automatic
*ex)* when Python runs operations involving integers and floats, it implicitly converts integer types intoo floats, then completes the operation.

However, while Python's implicit type conversion works when using the + operator between strings and integers, it does not work between strings and floats.

**Loop**

continue vs pass - pass will still make the rest of the loop AFTER the pass run before the next iteration. continue will stop that iteration right there and move onto the next iteration immediately.

#### Procedural Programming
- writing step by step instructions 
- stepping stone to object oriented programming
- DRY - Don't repeat yourself
- Create functions that can be reused

#### Functional Programming
- Is a programming paradigm that utilizes functions for clean, consistent, and maintainable code
- does not change the data outside the scope of the function

**Pure function** - no effect beyond its own scope
Using pure functions will help make code cleaner, easier to debug, and easier to read.
X need to worry about accidentally changing an original/global value 

**Difference between map and filter function**
map function applies it to every item in the list.
filter function does the same, but it returns a list to items that were True for the given function

**List comprehension in python**
syntax for list comprehension: [<expression\> for x in <sequence\> if <condition\>]
list comprehension in Python is a concise way to create list
--> allows for the generation of a new list by applying an expression/condition to each item in an existing iterable

similarly, dictionary and set comprehensions are also available.
In dictionary comprehension, you can have two prepared list and use the zip() function to match a value to a key in the same order of the two lists. an example can be:
```python
# Lists
months = ["Jan", "Feb", "Mar", "Apr", "May", "June", "July", "Aug", "Sept", "Oct", "Nov", "Dec"]
number = [1,2,3,4,5,6,7,8,9,10,11,12]

d = {key:value for (key,value) in zip(number, months)}
```

#### Object Oriented Programming
- relies heavily on simplicity and reusability to improve workflow
- **Class** - defined with a 'class' keyword
- **Attributes** - variables of the class
- **Behavior** - functions of the class
- Instances of the classes are called **objects**
  - in other words, a class provides a blueprint for creating an object
- ex) class - employee, attributes - id, status 

##### OOP Principles
- **Inheritance** - creating a new class (child class/subclass) which is a derivative of an existing one (parent class/superclass)
- **Polymorphism** - the ability of a function to change its behavior when called by different objects 
- **Encapsulation** - Limiting access to method and variables by encasing them in a single unit of scope
  - prevent unwanted modifications, reduce errors
- **Abstraction**


- classes have the ability to combine data and functionality (values and functions in one class/defined under the same class)
- class definition, create new inst ance, initialize new instance
- Statements inside a class body get executed regardless of the instance creation. 
- A **decorator** is a function that takes another function as an input/as its argument and gives a new function as its output
- Sometimes class inheritence can get complicated --> then how to tell the relationships?
  - **Simple Inheritance** - one parent, one child class
  - **Multiple Inheritance** - more than one parent
  - **Multi-level Inheritance** - more than one chain of parents
  - **Hierarchical Inheritance** - several subclasses inherit from a common parent
  - **Hybrid Inheritance** - Mix of all the other inheritances

#### Method Resolution Order (MRO)
- Determines the order in which a given method or attribute passed is searched 