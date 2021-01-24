![Python Logo](python.jpg)

# **Python Cheat Sheet**

**Requirements:**  
&nbsp;&nbsp;&nbsp;&nbsp;1. Knowledge of a programming language

# Variables

```python
num = 12
name = "brave"
isMan = True     # 1
isWoman = False  # 0
list = [1, 23, "Haha"]
dict = {"Brave": 15, "John": 20}
tuple = (20, 10, "Hello!",)
```

# Functions

```python
def func_name(arg, default_arg=10, args*, kwargs**):
	...
	return 0
```

**args\***: (1, 2, 3, ...)  
**kwargs\*\***: {a="Hello", b="World!", c="Haha"}

# Comment

```python
# this is a comment

"""
	this is a multiline comment
"""
```

# Operators

```python
num = 10   # init num var with 10
num + 2    # sum with 2
num - 2    # subtraction with 2
num * 5    # multiply with 5
num / 2    # division with 2
num % 4    # division with 4 and return remaining
num ** 2   # power with 2
num < 10   # does 10 bigger than num?
num > 5    # does num is bigger than 5?
num = 100  # equal with 100
```

# if Statements

```python
age = 19

if age >= 150:  # check if age is bigger than or equal with 150
	print("Please Enter Valid Age!")
elif age >= 18: # check if age is bigger than or equal wiht 18
	print("You can Enter!")
else: # if not run this statement
	print("You cant Enter!")
```

# for Loops

```python
for i in ["hello", "world"]:  # iterate ["hello", "world"] and print the members of list
	print(i)
```

# while Loop

```python
count = 0

while count <= 10:  # run this commands for 10 times
	print(count)
	count += 1
```

# Error Handling

```python
try:
	i = "0"
	i += 1
except:
	print("Type Error!")
else:
	print("if excepct section doesn't run this section wil run.")
finally:
	print("This section will run anyway!")
```

# Raise Errors

```python
try:
	raise SyntaxError
except SyntaxError:
	print("This is a Syntax Error!!!")
```

# Classes

```python
class MyClass(InheritanceClass):
	def __init__(self, name):
		# This method runs when an object creates from this class
		self.name = name
		...
	def sayhello(self):
		print(f"Hello {name}!")

myobj = MyClass(name="brave")
myobj.sayhello()
```

# Attachment

## Error Types

+ BaseException
  + SystemExit
  + KeyboardInterrupt
  + GeneratorExit
  + Exception
    + StopIteration
    + StopAsyncIteration
    + ArithmeticError
      + FloatingPointError
      + OverflowError
      + ZeroDivisionError
    + AssertionError
    + AttributeError
    + BufferError
    + EOFError
    + ImportError
      + ModuleNotFoundError
    + LookupError
      + IndexError
      + KeyError
    + MemoryError
    + NameError
      + UnboundLocalError
    + OSError
      + BlockingIOError
      + ChildProcessError
      + ConnectionError
        + BrokenPipeError
        + ConnectionAbortedError
        + ConnectionRefusedError
        + ConnectionResetError
      + FileExistsError
      + FileNotFoundError
      + InterruptedError
      + IsADirectoryError
      + NotADirectoryError
      + PermissionError
      + ProcessLookupError
      + TimeoutError
      + ReferenceError
      + RuntimeError
        + NotImplementedError
        + RecursionError
      + SyntaxError
        + IndentationError
          + TabError
      + SystemError
      + TypeError
      + ValueError
        + UnicodeError
          + UnicodeDecodeError
          + UnicodeEncodeError
          + UnicodeTranslateError
      + Warning
        + DeprecationWarning
        + PendingDeprecationWarning
        + RuntimeWarning
        + SyntaxWarning
        + UserWarning
        + FutureWarning
        + ImportWarning
        + UnicodeWarning
        + BytesWarning
        + ResourceWarning

## Built-in Functions

```python
# print 'Hello World!' on screen
print("Hello World!")
# get the age and save it in age var
age = input("Enter your age: ")
# return the type of "10"
type("10")
# converts "20" to integer type
int("20")
# converts 10 to string type
str(10)
# converts hello to list type
list("hello")
# converts 1 to boolean type
bool(1)
# creates dictionary with given data
dict(name="Brave", lang="FA")
# return the length of given string
len("Python Language!")
```

## Magic Methods

| Method    | Description                 |
| :-------: | :-------------------------: |
| __init__  | Run when initialize         |
| __new__   | Run when new object creates |
| __del__   | Destructor method           |
| __str__   | Called with str() func      |
| __int__   | Called with int() func      |
| __float__ | Called with float() func    |
| __add__   | Called with + operator      |
| __sub__   | Called with - operator      |
| __mul__   | Called with * operator      |
