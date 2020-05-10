# Introduction
### What will you learn?
- Basic functional programming structure
- Python data types and data structures and their manipulation
- Arithmetic Operators
- Control Flow
- Input prompts
- Loops
- Function declaration and built-in functions.
- Code Documentation and function Documentation
- Work with imported modules
- Learn how to use the built-in re, socket, and requests modules
  - The re module for compiling and using regular expressions.
  - The socket module for creating client-server sockets.
  - The requests module for constructing and sending HTTP requests.
- Cool Python Features

### What is Python?
Python is an interpreted, object-oriented, dynamically typed, and high-level programming language. Python was created by Guido van Rossum in 1991 and was developed for writing readable code and creating programs with fewer lines of code. Python is one of the top three languages in the world and has gained most of its popularity in the fields of artificial intelligence, backend web development, and data science. Python is most commonly used in cybersecurity for scripting practices which means it is used for automating tasks that would normally require step-by-step operations performed by a human. One important feature of Python to understand is that it is an interpreted language as opposed to compiled. Interpreted languages differ from compiled languages in the way that they are converted into a language that a computer can understand. Interpreted languages rely on an "interpreter" to interpret every line of code into machine processable syntax. Compiled languages perform a more rigorous phase-oriented process which include the following components: a preprocessor, a compiler, a assembler, and a linker. To read more about compiled languages, check out [this](https://www.youtube.com/watch?v=GExnnTaBELk&list=LLzN3gxCWCmr3Bbj_EBLE1SQ&index=22&t=0s) youtube video. Now that we have learned about what Python is and some of its characteristics, let's get into coding.

**Note**: Python 3.6+ is recommended for following all steps of this tutorial to avoid producing errors.

# Hello, World!
Hello world programs are essentially the first program a you would learn how to write when learning a programming language. So let's stick to the tradition and begin writing our "Hello, World!" program in Python.

```python
print("Hello, World!")
```
Running the code above will print out "Hello, World!" to the console, and can be ran by prefixing the name of the file that you have saved this code into with the word python - `python yourFileName.py`. All Python files you create need to be saved with the `.py` extension. The `print()` function used is a built-in Python function that prints data out to a console.


# Comments in Python
Comments are useful in Python and in other programming languages for understanding what a program is doing and can help guide others who are trying to understand your programs logic. Comments can also save you time when refering back to programs you have written. Here are the three types of comments in Python:
```python
# This is a single line comment.

'''
This
is
a
multi-line
comment.
'''

"""
This
multi-line
comment
works
exactly as
the one
above.
"""
```
Documenting our "Hello, World!" program might look something like this:
```python

# print "Hello, World!" to the console
print("Hello, World!")
```

# Data Types: string, integer, boolean, and float
Strings, integers, booleans, and floats are all data types in Python which are all used to represent data. 

**Strings**
  - Strings are a sequence of characters.
  - Strings are immutable which means you cannot overwrite a specific character of a strings, instead you would have to declare a completely different string.
  - 
  ```python
  Ex.
  # Any statement surrouned by double or single quotes are considered strings.
  Strings: "I love Python", 'I love Python' 
  # Both of the strings represented above are treated the same in Python.
  ```
  - Unlike many programming languages that support character data types, a character in Python is simply a string with a length of 1.
  ```python
  # This are characters, but really there just strings of length 1.
  Characters: "A" or 'a'
  ```
  
**Integers**
  - Integers are any whole numbers, both negative and positive.
  ```python
  Ex.
  # The following values are all valid integers.
  Integers: 1, 5, 2020, -3452, 0
  ```
  
**Booleans**
  - Booleans are logical data types that store represent only two values.
  ```python
  Ex.
  # Booleans are very useful for your programs control flow.
  Booleans: True, False
  # Note: Booleans must be capitalized in Python.
  ```
  
**Floats**
  - Floats represent real numbers and contain decimals to distinguish fractional and integer parts.
  ```python
  # Floats are mostly used for mathematical purposes.
  Floats: 0.1, 3.3, 5324.172, .77
  ```

# Data Structures: list, dict, tuple, and set
Data structures are a collection of data types. You use data structures to store data that are revelant to each othere, like a list of dates or IP addresses. Python is a dynamically typed language and therefore elements within any data structure can contain different data types. This means, for example, that creating a list with floats, strings, and integers is allowed in Python data structures. In statically typed languages, data structures can only store data that a declared data structure was determined to store. For example, in C++, arrays (C++'s version of lists) can only contain elements of the same data type: int, float, string, boolean.

**Lists**
- Lists can store any data type including other data structures. 
- Lists support indexing which means that elements are ordered and can be addressed using a unique index identifier.
- Lists are also mutable meaning that the elements within a list can be changed if they are mutable types.
```python
Lists: ["A string", 365.00, 7, True]
```

**Dicts**
- Dictionaries are a unique that data structure that use a key-value pair in order to distinguish every items.
  - dictionary keys must be an immutable type.
- Dictionaries, like lists, are mutable which means you can change a particular item within any given dictionary, if the item is mutable.
- In Python 3.6+, dictionaries preserve their order which means that items we insert into a dictionary can be expected to be at the location we designated them to be in.
- Dictionary items can be accessed using a specific syntax which we will discuss later.
```python
Dict: {"eye_color": "brown", 1: "A number", "male": True}
```

**Tuples**
- Tuples are immutable data structures which means there values cannot be altered and we cannot add new elements to them.
- Tuples are ordered thus elements can be accessed using indexes.
```python
Tuple: ("brown", 1999, 6.2)
```

**Sets**
- Sets store immutable data types: tuples, strings, ints, floats, bool
- Sets do not store duplicate values.
- Sets do not have ordering which means we can't use index notation to extract individual elements from a set.
```python
Set: {"John Wick", 20, True}
```

### Data Structure Declaration Syntax

|**Data structure**|**Declaration**|
|-------|-------|
|List|`[] or list()`|
|Dict|`{} or dict({})`|
|Tuple|`() or tuple()`|
|Set|`{} or set()`|


# Variables
Variables are used in programming languages to store data and are given names to better understand what the stored data represents.
Here are some variable declarations in Python using data types and data structures discussed earlier:
```python
"""
***********************************************
The "=" sign is called the assignment operator
and is used to declare variables.
***********************************************
"""

# Both ways of declaring a variable of type string.
name = "John Wick"
# OR
name = 'John Wick'

# This is a variable storing an integer.
age = 20

# This is a variable storing a float.
pi = 3.14

# This is a variable storing a boolean value.
male = True

# This is a variable storing a list.
my_list = ["John Wick", 20, 3.14, True]
# SAME AS
my_list = list("John Wick", 20, 3.14, True)

# This is a variable storing a dict
my_dict = {"name": "John", "age": "20", "male": True}
# SAME AS
my_dict = dict({"name": "John", "age": "20", "male": True})

# This is a variable storing a tuple.
my_tuple = ("John Wick", 20, True)
# SAME AS
my_tuple = tuple("John Wick", 20, True)

# This is a variable storing a set.
my_set = {"Alice", "alice"}
# SAME AS
my_set = set("Alice", "alice") # Note that "Alice" is different than "alice".
```

## More on Variables
- Variables are case-sensitive
  ```python
  name = "John" 
  # AND
  naMe = "John"
  # Are to different variables.
  ```

- Variable naming conventions
  ```python
  """ VALID """
  my_name = "Alexis"
  name0 = "Alexis"
  n00b = "Alexis"
  _my_name = "Alexis"

  """ INVALID """
   # Variables should not begin with numbers or special characters, besides underscore.
  0name = "Alexis" # BAD
  # Can't create number variables.
  1 = "Student" # BAD
  *name = "Mike" # BAD
  ```

- Variable names should be descriptive for readability
  ```python
  this_is_my_name = "Alexis"
  days_in_a_year = 365
  ```
  
- Variables should not match built-in keywords
  ```python
  """
  List of built-in keywords:
  and       del       from      not       while    
  as        elif      global    or        with     
  assert    else      if        pass      yield    
  break     except    import    print              
  class     exec      in        raise              
  continue  finally   is        return             
  def       for       lambda    try
  """

  # Ex.
  class = "some class" # This is invalid because python already uses this variable for something else.
  ```
  
- After declaring a variable with some data, the variable name can be used to referrence it's data
  ```python
  pi = 3.14

  print(pi) # We use the variable "pi" to retrieve the value 3.14 and print it out.

  # Output:
  # 3.14
  ```
# Arithmetic Operators

- **+**  |  **+=**
  - the '+' operator can be used to add integers, floats, and to concatenate strings together.
  
    ```python
    i = 34 + 6
    f = 34.0 + 6.0
    s = "Hello," + " World!"
    ```
  - the "+=" is known as the addition assignment operator and it adds a value to a variable and assigns the result of the       operation to the variable that was manipulated.
  
    ```python
    i = 5
    i += 5 # Same as i = 5 + 5
  
    s = "Hello,"
    s += " World!" # Same as s = "Hello," + " World!"
    ```
  
- **-**  |  **-=**
  - the '-' operator can be used to subtract integers, floats and is also used to define negative numbers.
    ```python
    i = 12 - 10
    f = 17.4 - 5.4
    n = -20
    ```
  - the '+=' operator is known as the subtraction assignment operator and it subtracts two values and assign the value to a variable.
    ```python
    i = 12
    i -= 10 # Same as i = 12 - 10
    ```
    
- **\***  |  **\*=**
  - the '*' operator is used for multiply two numbers and 
    ```python
    
    ```
  - the '*=' operator is known as the multiplication assignment operator and it multiply integers, floats , and it is also used to multiply a given sequence type multiple times. 
- **%**  |  **%=**
  - the '%' operator is used to performing modular arithmetic. This operator essentially checks how many times a number goes into another number and then returns the remainder. The modulus operator is commonly used to check if a number is even or odd. A number is said to be even if 2 goes into that number perfectly without a remainder. A number is said to be odd if 2 goes into the number a certain number of times with a remainder of 1.
    ```python
    """
    i would be equal to zero in this statement 
    because 2 goes into 10 exactly 5 times
    without a remainder. Because we are checking 
    the mod 2 of this and the remainder is 0 know the
    number is even.
    """
    i = 10 % 2
    
    """
    in this example, i would be equal to 1
    because 2 goes into 11 5 times with a REMAINDER
    of 1. Because we are checking the mod 2 of this
    and the remainder is 1 we know the number is odd.
    """
    i = 11 % 2
    ```
  - the '%' operator is known as the modulus assignment operator and perform the same function as the '%' but it also assigns the return value to a given variable.
- **==**  |  **>=**  |  **<=**
  - the '==' operator is used to check if two values are equal.
    ```python
    i = 10
    print(i == 2) # Will print False because 10 does not equal 2
    
    # Output:
    # False
    ```
  - the '>=' operator symbolizes "greater than or equal to" evaluation. The '>' must come before the '='.
    ```python
    i = 10
    j = 5
    """
    The following line will print True because one
    of the conditions of the `>=` operator is True:
    10 is greater than 5.
    """
    print(i >= j)
    
    
    # Output:
    # True
    ```
  - the '<=' operator symbolizes "less than or equal to" evaluation. The '<' must come before the '='.
    ```python
    i = 10
    j = 5
    """
    The following line will print False because no 
    conditions of the operator `<=` are satified.
    10 is neither less than nor equal to 5.
    """
    print(i <= j)
    ```
**Note**: there are other operators but they will not be mentioned here. For more operators, visit this [link](https://www.tutorialspoint.com/python/python_basic_operators.htm).

# User Input
User input is important if your program relies on external data that a user may need to provide. To retrieve data from a user while during program run-time, we use the keyword *input*.
```python
# This will stop the execution of the program and wait for input.
# All inputs are automatically stored as strings.
# Values of non string type needed to converted later.

# Get input without a message prompt.
name = input()

# Get input with a message prompt.
name = input("Please enter your name: ")
```

# Built-in Functions
The following examples will demonstrate some of Python's built-in functions which will or can be useful to accomplish any given task. Python's built-in functions will allow you to do things such as get the length of a list, convert a variable, if allowed, to another data type (also known as type conversion/casting), and sort items. To invoke (fancy way for saying call or use) any function we must use opening paranthesis `(`, followed by the data in which we will pass to the function, and then a closing paranthesis `)`. Here are some built-in function examples:

**len**

len will return a number representing the number of characters within an iterable object (lists, tuples, and strings). The len is useful when performing loops. 
```python
name = "John"

len_of_name = len(name)

print(len_of_name)

# Output:
# 4
```

**sorted**

The sorted function returns a sorted list of an iterable object (lists, tuples, and strings). 
```python
my_list = [5, 4 , 7, 8, 2]

sorted_list = sorted(my_list)

print(sorted_list)

#Output:
[2, 4, 5, 7, 8]

"""
Most of Python's built-in functions 
will have specific options that we can 
pass in as arguments. Here is one argument
I will provide to the sorted function to return
a reversed sorted list (highest to lowest):
"""
my_list = [5, 4 , 7, 8, 2]

sorted_list = sorted(my_list, reverse=True)

print(sorted_list)

#Output:
[8, 7, 5, 4, 2]
```

**str, int, float, bool**

These three functions are to used to convert other data types into values defined by their names.
```python
"""
We can use Python's built-in type() function
to check the data type of a particular variable.
"""

i = 25

str_i = str(i)

print(type(str_i))

print(str_i)

# Output:
# <class 'str'>
# 25

# The "<class 'str'>" means the variable is of type string
# which means we converted the integer 25 into a string.

string = "77"

# Casting "77" into the integer 77
integer_from_string = int(string)

print(type(integer_from_string))

print(integer_from_string)

# Output:
# <class 'int'>
# 77

# The "<class 'int'>" means the variable is of type int
# which means we converted the string "77" into an integer.

i = 34

f = float(i)

print(type(f))
print(f)

# Output:
# <class 'float'>
# 34.0

# The "<class 'float'>" means the variable is of type float
# which means we converted the integer 34 into a float with 
# the value of 34.0

"""
***************************************
The bool function is a bit more complex
than the other type casting functions
previously demonstrated. The following values
will return a value of false when using the
bool function:
- None
- False
- Any value equal to 0
- Empty sequences and dictionaries.

The following will return True when using
the bool function:
- True
- any sequence (list, tuple, string) that is not empty
- any variable that contains an object
 that is not one of the elements in the previously
 listed False values.
***************************************
"""

my_list = []
name = "Alice"
i = 36
male = False
my_dict = {}

print(bool(my_list))
print(bool(name))
print(bool(i))
print(bool(male))
print(bool(my_dict))

# Output:
# False
# True
# True
# False
# False
```

**bytes**

The bytes function converts passed in data into a byte string of a specified encoding. Byte strings are identified by a 'b' preceding a string.
```python
name = "Neil"

byte_string = bytes(name, "utf-8") # Convert string into UTF-8 encoded byte object.

print(byte_string)

# Output:
# b'Neil'
```

**max, min**

The purpose of these functions is self-explanatory. Finding the maximum or minimum values in a compatible object.
```python

my_list = [34, 5, 2, 99, 58]

print(max(my_list))
print(min(my_list))

# Output:
# 99
# 2
```

**open**

The open function is utilized in Python for opening files in different modes that might be useful for your file operations.

|**mode**|**definition**|
|-------|-------|
|`r`|read from file only|
|`rb`|read from file in binary only|
|`r+`|read and write to file|
|`rb+`|read and write to file in binary|
|`w`|write to file only. Overwrites existing file or creates new one|
|`wb`|write to file in binary only. Overwrites existing file or creates new one|
|`w+`|write and read to file. Overwrites existing file or creates new one|
|`wb+`|write and read to file in binary. Overwrites existing file or creates new one|
|`a`|append data to file only|
|`ab`|append data to file in binary only|
|`a+`|append and read to and from file. Will create the file if it does not exist|
|`ab+`|append and read to and from file in binary. Will create the file if it does not exist|

---
```python
# Here we are opening a file in write mode.
f = open("somefile.txt", "w")

# The open function returns a file object
# which has methods (functions) that can be
# called. Because we've opened the file in
# write mode, lets use the write function
# to actually write to the file.

# Write to file using write method.
f.write("Hello, I am writing to this file")

# It is good practice to always close your files.
f.close()

# ------------------------------------------------

# Now lets open the samefile in read mode.
f = open("somefile.txt", "r")

# Let us read the data from the file which we 
# wrote into it.
data = f.read()

# Print the data obtained from the file.
print(data)

# Close the file.
f.close()
```

**print**
We've seen the print function being used many times, so let's get a better understanding of this commonly used function.
```python
# As mentioned before, the print function allows 
# us to display data to the console. 
print("This is a test")

# Seperated variables or defined strings with
# commas will automatically put spaces in between
# these elements.
print("This", "is", "a", "test")

# The print statement also appens a '\n' character
# to the end of your printed data which means 
# the cursor moves to the beginning of the 
# next line. We can change this though using
# a keyword argument called "end".
print("This", end="|")
print("is", end="|")
print("a", end="|")
print("test", end="|")

# VS

print("This")
print("is")
print("a")
print("test")

# Final Output:
# This is a test
# This is a test
# This|is|a|test
# This
# is
# a
# test
```

**range**

The range function returns an immutable sequence of numbers that we can use to create a range of numbers. The first element of any indexable data type or data structure is at index 0. This is because programming languages used zero-indexed based sequences. This means if we wanted to access the first element in `my_list = ['a', 'b', 'c']` we would do `my_list[0]`. 
```python
# Produce a range of numbers from 0 to 9.
# The value passed in as an argument is
# not included within the range of numbers
# because of 0-based indexing.
r = range(10)

# If we were to loop over this range
# and print the value of every number:
for i in r:
  print(i)
  
# Output:
# 0
# 1
# 2
# 3
# 4
# 5
# 6
# 7
# 8
# 9

"""
As shown above, the first number is 0 and
the last number is 9 because the value 10
passed as an argument to the function "range" 
is non-inclusive.
"""
```

# Control Flow
What is control flow?

```python
"""
**************************************************
- The "==" sign is used to check if two data types
or data structures are equivalent.
- The "if", "elif", and "else" are all keywords
used in controlling the flow of a Python program.
**************************************************
"""

name = "John"

if name == "John":
  print("Your name is John")
  
elif name == "Alice":
  print("Your name is Alice")
  
else:
  print("I do not know your name")
```

# Loops
```python
"""
*******************************************************
In python, the words "while", "for", "in", and "range"
can be a part of a loop operation. Note: "for",
"in" are used in conjunction and "range" is used 
by "while loops" and "for loops" interchangeably.

Indents in Python indicate block of codes. In any loop
we create must indent all of the steps in which we want
to perform within the of the loop.
*******************************************************
"""

# Ex. While Loop:
number = 1

# Performing some operation repeatedly until a condition is satisfied.
while number < 10:
  print(number)

# Ex. For Loop:
# For loops are great for repeatedly performing some operation a determined number of times.
for i in range(10)
  print(i)
```

**While loops**

While loops are excellent to use when you want to perform a series of steps while a given condition is true. While loops can also be used to create infinite loops when a condition is not provided or unknown. 
```python
"""
************************************************
When a condition to a while loop is given, there
will always be some variable that will be 
used to evaluate the condition for a loop
after each iteration.
************************************************
"""
# Ex.
counter = 0

while counter < 10:
  print("Hello")
  counter += 1
print("While loop finished!")

"""
Output:
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
While loop finished!

Hello was printed out 10 times because
the initial value of the variable counter was 0; 
This means the initial condition that was being
evaluated was is "0 < 10", and 0 is less than 10 so the 
action within the loops code block was executed. The
variable counter is then incremented by 1.
This evaluation occurs recursively until the 
condition becomes False when the variable counter equals 10 and
the condition being checked becomes "10 < 10" which returns
False. This exits the loop block and continues on to
the next line of code which in this case is print("While loop finished!")
"""
```

**For loops**

For loops should be used when you know the number of times you want to perform a given task.
```python
"""
**********************************************
For loops are excellent for when you know the 
number of times in which you would like to 
execute code. We can also use for loops
to iterate over any sequence type.
**********************************************
"""
# Looping over a range of numbers
for i in range(10):
  print(i)

# Looping over a string.
name = "John"
for letter in name:
  print(letter)

# Looping over a list.
list_of_names = ["Neil", "Alice", "John"]
for name in list_of_names:
  print(name)
  
"""
Output:
0
1
2
3
4
5
6
7
8
9
J
o
h
n
Neil
Alice
John

- In the first loop, we are iterating over a range of
numbers, 0 through 9, and printing each number.
- In the second loop, we are iterating over a string
which is a sequence type and printing each character in
the string.
- In the final loop, we are iterating over a list and
printing each item of the list.
"""
```
# Function Declaration
Functions are an important part of any programming language and they help you break down the tasks in your program into cohesive blocks of code that makes sense to the context of your program. Functions are created to avoid repetitive code blocks, making your programs simpler to read and understand.
```python
"""
How to declare a function:
def print_a_name(name):
    # Your code goes here...
    
We used to "def" keyword to "define" a
function called print_a_name which will take
in an argument in which we called name.
Let's finish this example function declaration:
"""

def print_a_name(name):
  print("Your name is", name)

n = "Frank"
print_a_name(n)

# Output:
# Your name is Frank

"""
We declared the function print_a_name
which will take name as an arguments.
The purpose of print_a_name is to print
"Your name is" followed by a name that
was passed as the argument. So we declared a 
variable, n, with a string of "Frank". We then 
invoked the function print_a_name by writing
the name of the function followed by opening and
closing parathesis and the variable n in between
them to signify that the argument we want to pass
into print_a_name is n.
"""
```

# PEP8 Documentation


# Importing Modules
Importing modules into your python programs will extend the functionality of your programs by including other useful tools from programs that Python has provided or that other programmers have created. Here are some ways of importing modules and import specific items from any particular module.
- basic syntax for importing a module:
  ```python
  import sys
  
  # The dir returns a list of the attributes and methods of any object (functions, modules, strings, lists, dictionaries,
  # etc)
  print(dir(sys))
  
  """
  Output:
  ['__breakpointhook__',
  '__displayhook__',
  '__doc__',
  '__excepthook__',
  '__interactivehook__',
  '__loader__',
  '__name__',
  '__package__',
  '__spec__',
  '__stderr__',
  '__stdin__',
  '__stdout__',
  '__unraisablehook__',
  '_base_executable',
  '_clear_type_cache',
  '_current_frames',
  '_debugmallocstats',
  '_framework',
  '_getframe',
  '_git',
  '_home',
  '_xoptions',
  'abiflags',
  'addaudithook',
  'api_version',
  'argv',
  'audit',
  'base_exec_prefix',
  'base_prefix',
  'breakpointhook',
  'builtin_module_names',
  'byteorder',
  'call_tracing',
  'callstats',
  'copyright',
  'displayhook',
  'dont_write_bytecode',
  'exc_info',
  'excepthook',
  'exec_prefix',
  'executable',
  'exit',
  'flags',
  'float_info',
  'float_repr_style',
  'get_asyncgen_hooks',
  'get_coroutine_origin_tracking_depth',
  'getallocatedblocks',
  'getcheckinterval',
  'getdefaultencoding',
  'getdlopenflags',
  'getfilesystemencodeerrors',
  'getfilesystemencoding',
  'getprofile',
  'getrecursionlimit',
  'getrefcount',
  'getsizeof',
  'getswitchinterval',
  'gettrace',
  'hash_info',
  'hexversion',
  'implementation',
  'int_info',
  'intern',
  'is_finalizing',
  'maxsize',
  'maxunicode',
  'meta_path',
  'modules',
  'path',
  'path_hooks',
  'path_importer_cache',
  'platform',
  'prefix',
  'ps1',
  'ps2',
  'ps3',
  'pycache_prefix',
  'set_asyncgen_hooks',
  'set_coroutine_origin_tracking_depth',
  'setcheckinterval',
  'setdlopenflags',
  'setprofile',
  'setrecursionlimit',
  'setswitchinterval',
  'settrace',
  'stderr',
  'stdin',
  'stdout',
  'thread_info',
  'unraisablehook',
  'version',
  'version_info',
  'warnoptions']
  """
  ```
- importing a module and utilizing the **as** keyword to use a specified name for referring to the module as opposed to the original name of the module:
  ```python
  import sys as s
  
  # sys.argv stores the arguments that were passed to the Python file currently executed.
  command_arguments = s.argv
  print(command_arguments)
  
  """
  Example:
  ./test.py hello world 1 2 3
  
  Output:
  ["hello", "world", "1", "2", "3"]
  """
  ```
- importing a particular function or class from another module is done using the **from** keyword:
  ```python
  from sys import argv
  
  # print the name of the current file.
  # Note: if shebang was used to specify the Python intepreter,
  # you'll see a **./** preceding the name of the file.
  print(argv[0])
  
  """
  Example:
   python test.py
  
  Output if using python3 to directly run file:
  test.py
  
  Output if using a shebang to direct the terminal to execute the file as a Python file:
  ./test.py
  """
  ```

# The re, socket, and requests Module

### re
The re module is used for compiling and providing regular expression searching within your program. Regular expressions are a sequence of characters that define a specific search pattern. For an excellent regular expression cheat sheet, follow this [link](https://devhints.io/regexp). Let's look at some regular expressions that you will most likely use in cybersecurity: 
```python
import re

"""                       Regular Expressions                         """
#------------------------------------------------------------------------
FULL_URL_REGEX = re.compile(r"https?://(www\.)?([a-zA-z-]+)(\.\w+)")
EMAIL_REGEX = re.compile(r"[a-zA-Z-_]+@[a-zA-Z-_]+\.[a-zA-Z]+")
PHONE_NUMBER_REGEX = re.compile(r"(?[0-9]{3})? [0-9]{3}( -)?[0-9]{4}")
IP_REGEX = re.compile(r"[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}")

# Let's break down each regular expression shown above.



```

### socket
The following example consists of the methods we use to create a client using the socket module:
```python
# Import the socket module
import socket as s

# IP address and port of the server we will be connecting to
IP = "127.0.0.1"
PORT = 1234

# Number of bytes to receive from server at any given point
BYTES = 1024

# Creating a socket
sock = s.socket(s.AF_INET, s.SOCK_STREAM)

# Connecting to server
# Note: the socket.connect() method
# expects a tuple containing the IP address
# and port number of the server
sock.connect((IP, PORT))

# Receiving data from our server
# and decode the bytes into utf8 text
sock.recv(BYTES).decode("utf-8")

# Message to send to server
message = "Hello server!"

# Send message to clients
sock.send(message.encode("utf-8"))

# Close the socket 
sock.close()
```

The following example consist of the methods we use to create a server using the socket module:
```python
# Import the socket module
import socket as s

# IP and port number to bind our socket to
IP = "127.0.0.1"
PORT = 1234

# Number of bytes to receive from server at any given point
BYTES = 1024
# Creating our socket
sock = s.socket(s.AF_INET, s.SOCK_STREAM)

# Binding our server to an IP address and port number
sock.bind((IP, PORT))

# Tell our server to start listening for incoming connections
sock.listen()

# Receive data from client machines
# and decode bytes received into utf8 text
sock.recv(BYTES).decode("utf-8")

# Message to send to clients
message = "Hello clients!"

# Send message to clients
# Note
sock.send(message.encode("utf-8"))

# Close the socket
sock.close()
```

### requests
The requests module is a great tool for sending HTTP requests to a website. Here are some of the properties and methods commonly used for the requests module. **Note**: You will have to install the requests module because it is not a built-in Python module. To install it on Linux, type `pip install requests` in your terminal and let the magic happen. If you are on Windows you need to make sure you have Python installed and then open up a command prompt as administrator and type `pip install requests`.
```python
import requests

URL = "www.google.com"

# Make a GET requests to www.google.com
resp = requests.get(URL)

# Check the status code of the requests
print(resp.status_code)

# Get the response headers
print(resp.headers)

# Return a JSON object if the response contained
# JSON data
resp_json = resp.json()

# Get the HTML content received from the response
site_HTML = resp.text
print(site_HTML)

"""
Make a POST requests to www.google.com
and send data 
Note: the same properties from above
are also accessible by the object returned
from the .post() function.
"""
post_req_resp = requests.post(URL, data={"name": "test"})

print(post_req_resp.status_code)
print(post_req_resp.headers)
print(post_req_resp.json())
print(post_req_resp.test)
```

# Cool Python Features

### F strings

F-strings are Python's new way of formatting strings. 
```python
name = "Neil"
age = 25
height = 6.2

print(f"My name is {name} and I am {age} year's old. I am also {height} ft tall.")

# Output:
# My name is Neil and I am 25 years old. I am also 6.2 ft tall.
```

### Context managers

Context managers in Python are using for handling resource that require opening and closing operations such as open a file or creating a socket. The "with" keyword is used for context managers and essentailly any class that contains the \__enter__ and \__exit__ dunder (double underscore) methods support context management.
```python
import socket

"""
Here is an example of how we would use a context manager to open and close a socket.
"""
with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
  pass
```

### Reversing a sequence type with slice notation

```python
name = 'John'
reversed_name = [::-1]
print(name)

list_of_chars = ['a', 'b', 'c', 'd']
reversed_list_of_chars = my_list[::-1]
print(reversed_list_of_chars)
```
### List, dict, and set comprehensions

List, dictionaries, and sets can all be created using a one-line statement known as a list|dict|set comprehension. The creation of list, dicts, or sets that require complex control flow should not be created with comprehensions because the readability of comprehension can get complicated after a certain number of operations.
```python
list_of_chars = [c for c in ['c', 'b', 'a']]
```

# About the Author
Alexis Rodriguez is a cybersecurity professional with an fondness for the art of programming. He studied computer science at Hunter College where he learned how to program in C++ and Python, and graduated Fullstack Cyber Bootcamp where he gained his cybersecurity foundation. His favorite quote is: "It is the knowledge of knowing that I am going to die that creates the focus that I bring to being alive." - *Neil Degrasse Tyson*.
