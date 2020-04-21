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
Documenting the "Hello, World!" program might look something like this:
```python

# This line will print "Hello, World!" to the console
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
1. **+**, **+=**
  - the "+" operator can be used to add integers, floats, and to concatenate strings together.
    ```python
    i = 34 + 6
    f = 34.0 + 6.0
    s = "Hello," + " World!"
    ```
  - the "+=" is known as the addition assignment operator and it adds a value to a variable and assigns the result of the operation to the variable that was manipulated.
  ```python
  i = 5
  i += 5 # Same as i = 5 + 5
  
  s = "Hello,"
  s += " World!" # Same as s = "Hello," + " World!"
  
  ```
2. **-**, **-=**

3. *****, ***=**

4. **/**, **/=**

# User Input
User input is important if your program relies on external data that a user may need to provide. To retrieve data from a user while program run-time, we use the keyword *input*.
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
|`a`|append data to file|
|`ab`|append data to file in binary|
|`a+`|append and read. Will create the file if it does not exist|
|`ab+`|append and read to and from file in binary. Will create the file if it does not exist|

```python
"""
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

# Close the file we opened.
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
********************************************
When a condition to a while is given, there
will always be some variable that will be 
used to evaluate the condition for a loop
after each iteration.
********************************************
"""
# Ex.
counter = 0

while counter < 10:
```

**For loops**
For loops should be used when you know the number of times you want to perform a given task.
```python

```

# About the Author
Alexis Rodriguez is a cybersecurity professional with an adoration for the art of programming. He studied computer science at Hunter College where he learned how to program in C++ and Python, and graduated Fullstack Cyber Bootcamp where he gained his cybersecurity foundation. His favorite quote is: "It is the knowledge of knowing that I am going to die that creates the focus that I bring to being alive." - *Neil Degrasse Tyson*.
