How programmme get converted to executable code in different languages?
<img width="724" height="365" alt="image" src="https://github.com/user-attachments/assets/8bd09ea2-3acc-455e-9cd0-901d5bbfefab" />

--> In Python, the component that converts your .py source code into .pyc bytecode is simply called the Python Compiler. In modern Python (3.x), you won't usually see .pyc files cluttering your main folder. Instead, Python creates a folder named __pycache__. <br>
--> That bytecode is then fed into the Python Virtual Machine (PVM), which is the heart of CPython. The PVM is the "interpreter" that actually executes the instructions.

# <b>Variables: </b> define varaible type - pvm doesn't care of this type definition, so you would store String into int type

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


<b>list </b> -> define with sqare bracket []
  - list is immutable
<b>tupple </b> -> define with bracket ()
  - tupple is mutable
<b>set </b> -> define with  bracket {}
  - set doesn't gurranty the order
  - set doesn't allow duplicate value
<b>dictionary </b> -> define with bracket {},  dict = {key:value, key1:value1}
  - its a key value pair
  - keys are always unique, if you enter duplicate latest one will be in consider
  - below are method to access this
    dict[key1] - reurn corresponding value
    dict.get(key1, 'Not Available')
    del dict[key], dict.pop('key') - to delete or remove a pair
    dict.keys()
    dict.values()


<b> array </b> -> 
