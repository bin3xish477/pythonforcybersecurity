# Introduction to Python for Cybersecurity
## What will you learn?
- Basic functional programming structure
- Python data types and data structures and their manipulation
- Input prompts
- Function declaration and built-in functions.
- Code Documentation and function Documentation
- Work with imported modules
- Work with 2 important built-in modules: socket and requests
  - The socket module for creating client-server sockets.
  - The requests module for constructing and sending HTTP requests.
--------------------------------------------------------------------------------------------------------------------------
## What is Python?
Python is an interpreted, object-oriented, and high-level programming language. It was created by Guido van Rossum in 1991 and was developed for writing readable code and creating programs with fewer lines of code. Python is one of the top three languages in the world and has gained most of its popularity in the fields of artificial intelligence, backend web development, and data science. Python is most commonly used in cybersecurity for scripting practices which means it is used for automating tasks that would normally require step-by-step operations performed by a human. One important feature of Python to understand is that it is an interpreted language as opposed to compiled. Interpreted languages differ from compiled languages in the way that they are converted into a language that a computer can understand. Interpreted languages rely on an "interpreter" to interpret every line of code into machine processable syntax. Compiled languages perform a more rigorous phase-oriented process which include the following components: a preprocessor, a compiler, a assembler, and a linker. To read more about compiled languages, check out [this](https://www.youtube.com/watch?v=GExnnTaBELk&list=LLzN3gxCWCmr3Bbj_EBLE1SQ&index=22&t=0s) youtube video. Now that we have learned about what Python is and some of its characteristics, let's get into coding.

**Note**: Python 3.6+ is recommended for following all steps of this tutorial to avoid producing errors.
--------------------------------------------------------------------------------------------------------------------------
## Hello, World!
Hello world programs are essentially the first program a you would learn how to write when learning a programming language. So let's stick to the tradition and begin writing our "Hello, World!" program in Python.

```python
print("Hello, World!")
```
Running the code above will print out "Hello, World!" to the console, and can be ran by prefixing the name of the file that you have saved this code into with the word python - `python yourFileName.py`. All Python files you create need to be saved with the `.py` extension. 

## Comments in Python
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

## Data Types: strings, integers, booleans, and floats
Strings, integers, booleans, and floats are all data types in Python which are all used to represent data. 

**Strings**
  - Strings are a sequence of characters.
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
  
## Data Structures: list, dict, tuples, sets

## Variables
Variables are used in programming languages to store data and given names to better understand what data represents.
Here are some variable declarations in Python using data types discussed earlier:
```python
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
```

--------------------------------------------------------------------------------------------------------------------------

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
