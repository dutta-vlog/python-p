How programmme get converted to executable code in different languages?
<img width="724" height="365" alt="image" src="https://github.com/user-attachments/assets/8bd09ea2-3acc-455e-9cd0-901d5bbfefab" />

--> In Python, the component that converts your .py source code into .pyc bytecode is simply called the Python Compiler. In modern Python (3.x), you won't usually see .pyc files cluttering your main folder. Instead, Python creates a folder named __pycache__. <br>
--> That bytecode is then fed into the Python Virtual Machine (PVM), which is the heart of CPython. The PVM is the "interpreter" that actually executes the instructions.

# <b>Variables: </b> define variable type - pvm doesn't care about this type definition, so you would store String into int type

import typing <br />
-- Define a variable of type str<br>
z: str = "Hello, world!" <br><br>
-- Define a variable of type int<br>
x: int = 10 <br><br>
-- Define a variable of type float <br>
y: float = 1.23 <br><br>
-- Define a variable of type list <br>
list_of_numbers: typing.List[int] = [1, 2, 3] <br><br>
-- Define a variable of type tuple <br>
tuple_of_numbers: typing.Tuple[int, int, int] = (1, 2, 3) <br><br>
-- Define a variable of type dict <br>
dictionary: typing.Dict[str, int] = {"key1": 1, "key2": 2} <br><br>
-- Define a variable of type set <br>
set_of_numbers: typing.Set[int] = {1, 2, 3} <br><br>


- <b>list </b> -> define with sqare bracket [] : list is Mutable <br />
- <b>tupple </b> -> define with bracket () : tupple is Immutable <br />
- <b>set </b> -> define with  bracket {} <br />
  : set doesn't guarantee the order <br />
  : set doesn't allow duplicate value <br />
- <b>dictionary </b> -> define with bracket {},  dict = {key:value, key1:value1} <br />
  : it is a key value pair <br />
  : keys are always unique, if you enter duplicate latest one will be in consider <br />
  : below are methods to access this <br />
    dict[key1] - return corresponding value <br />
    dict.get(key1, 'Not Available') <br />
    del dict[key], dict.pop('key') - to delete or remove a pair <br />
    dict.keys() <br />
    dict.values() <br />
- <b> array </b> -> array is for a similar type of variable, list and tupple can have multiple type but not in array

# Functions and Arguments:
Arguments: <br />
  1. undefined arguments should be before the defined one
  2. *arg -> it actually takes all the extra values and creates a tupple
  3. **keyarg -> it takes all the extra values which are defined with argument name and creates a dictionary

<b>recursion </b>: you can set recursion limit by sys.setrecursionlimit(10) , and get using sys.getrecursionlimit() <br />
<b>higher-order function </b>: we can pass a function as argument to other functions, return them from functions, and store them in variables. <br />
<b>lambda function </b>: it's also called anonymous function, it has no name and don't need to define it using <b> def func_name(): </b> <br />
square = lambda x: x * x <br />
print(square(5)) <br />

# filter map reduce:
      nums = [1, 2, 3, 4, 5, 6] 
      evens = list(filter(lambda x: x % 2 == 0, nums)) 
      print(evens) # Output: [2, 4, 6]  

# inner function:
      def outer_func(): 
              print("I am inside outer function") 
      
              def inner_func(): 
                  print("I am inside inner function") 
      
              return inner_func 
      
      inner_func_ref = outer_func() 
      inner_func_ref() 
      
      ### output : 
      I am inside outer function
      I am inside inner function

# decorator:
    def my_decorator(func):
        def wrapper():
            print("Something is happening before the function is called.")
            func()  # This is your original function being called inside decorator
            print("Something is happening after the function is called.")
            return func()
        return wrapper

    @my_decorator
    def say_hello():
        print("Hello!")
    
    say_hello()


# Modules and packages:
In Python, a Module is simply a file containing Python code. It can define functions, classes, and variables. If you save a file named math_helpers.py, you have created a module named math_helpers.
Basically '.py' files are a Module, where we can write functions, classes or both.

    
# Special variable:
- <b> globals() </b> : returns all the global variable, including name, doc, package, file, etc <br />
- <b> __name __ </b> : value is __main __ when current file is the main runinng file, or module name when some other file is the main file and calling this file



# Object:
- **self** is always required in python as a first parameter in method, this is same as this in java. we can access instance method as well using **self.variable**
- **__init __()** method is not a constructor, it always gets called whenever object is created, in't called initializer method
- we can also create an object using **ClassName.__ new__(className)**, this time __init __() will not get called
- __ new __() is a constructor, it actually creates the object in memory.
- python actually calls both the methods

<img width="575" height="239" alt="Screenshot 2026-01-21 at 3 06 10 AM" src="https://github.com/user-attachments/assets/8f1c37b5-2334-4755-8108-6c1613972163" />

