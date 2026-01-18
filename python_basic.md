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


- <b>list </b> -> define with sqare bracket [] : list is Mutable \n
- <b>tupple </b> -> define with bracket () : tupple is Immutable \n
- <b>set </b> -> define with  bracket {} \n
  : set doesn't guarantee the order \n
  : set doesn't allow duplicate value \n
- <b>dictionary </b> -> define with bracket {},  dict = {key:value, key1:value1} \n
  : it is a key value pair \n
  : keys are always unique, if you enter duplicate latest one will be in consider \n
  : below are methods to access this \n
    dict[key1] - return corresponding value \n
    dict.get(key1, 'Not Available') \n
    del dict[key], dict.pop('key') - to delete or remove a pair \n
    dict.keys() \n
    dict.values() \n

- <b> array </b> -> array is for a similar type of variable, list and tupple can have multiple type but not in array

# Functions and Arguments
Arguments: \n
  1. undefined arguments should be before the defined one
  2. *arg -> it actually takes all the extra values and creates a tupple
  3. **keyarg -> it takes all the extra values which are defined with argument name and creates a dictionary

recursion : you can set recursion limit by sys.setrecursionlimit(10) , and get using sys.getrecursionlimit()


