# Python Fundamentals

## Topic Overview

### Introduction
- Course Overview
  1. Setting up your machine
  2. Data Types and Operators
  3. Strings and String manipulation
  4. Variables
  5. Collections
  6. Control Flow
  7. Loops
  8. Function


### Course Setup

- Python Installation - Mac
  - Please follow this link: [https://www.python.org/downloads/](https://www.python.org/downloads/)
- Python Installation - Windows
  - Please follow this link: [https://www.python.org/downloads/](https://www.python.org/downloads/)

- Pycharm Installation
  - Please follow this link: [https://www.jetbrains.com/pycharm/download/?section=windows](https://www.jetbrains.com/pycharm/download/?section=windows)

- First Python Project
   - Short Introduction of virtual environment
     - A virtual environment captures a local version within that folder (called venv) of Python itself
   - First Project: `print("Hello World!")`
     1. Create a new file by right-clicking on the folder, where you would like to store your file
     2. Select `New` and then `File`
     3. Enter the name of the File with the extension `.py` for Python: `hello_world.py`
     4. Type `print("Hello World!")` and click on the play button
     5. You should receive the following in your terminal:<br>
     ![print statement](https://github.com/SKaurGithub/data_402_python/assets/153448835/4800a790-0c0e-4b1e-a357-12cc483e4f88)

     Congratulations! You have written your first code!

- Commenting Code
  - It is important to add comments as this can help another person to understand your code
  - You can comment code in different ways:
    - Adding a hashtag at the start of your comment:<br>
    ![comment](https://github.com/SKaurGithub/data_402_python/assets/153448835/1c663ff3-433f-4c9a-a543-d6b26c49ef6a)
    - You can also add in-line comments:<br>
    ![in-line comment](https://github.com/SKaurGithub/data_402_python/assets/153448835/f60e5515-9c49-4891-8a03-2c459f29ee35)
    - You can also add multi-line string as this can be used as a comment as well:<br>
    ![multi line string](https://github.com/SKaurGithub/data_402_python/assets/153448835/b08b8616-6253-43cb-845c-5125954d11db)

    
  

### Data Types

- Data Types Intro
  - Integers/Floats:
    - Integers are whole numbers
    - Floats are decimal numbers
  - Strings:
    - Strings consist of a combination of characters
    - They always need to be in single or double quotes
  - Boolean:
    - Boolean can only store one of two values, namely True or False
    - Make sure to capitalise them as it will not be recognised as a boolean otherwise


- Numbers and Math Operators
  - Math Operators: `+`, `-`, `*`, `/`, `%`:
    - You can use these operators to conduct mathematical calculations with integers and floats
    - Please bear in mind that `10` and `"10"` is NOT the same. 
      `10` is an integer (whole number)
      `"10"` is a string -- in order to use a string for calculations, you will need to cast it into a integer `int()` or into a float `float()` first

  - Built-In Function: `type()`
    - This function will show you the type of your output:
    ![type()](https://github.com/SKaurGithub/data_402_python/assets/153448835/8f1b2949-fe4c-4559-b165-5f075addeb8e)
 ![output of type()](https://github.com/SKaurGithub/data_402_python/assets/153448835/adc8d656-5c4a-4f02-8238-711099f58a71)

    

- String Basics
  - Unicode Characters
    - The Python Interpreter does not see words like we do. It sees a group of Unicode characters put together in a particular sequence.
      Unicode is a standard for representing text in computers. It assigns a unique number to every character in every language, including symbols and emojis.
  - Indexing
    - This is useful if you would like to access a particular part of a string, list etc.
    - We use square brackets for this `[]`
    - The first character starts with the index `0` 
    - The first index is the starting index, which is included
    - The last index is the ending index, which is excluded<br>
      ![index example](https://github.com/SKaurGithub/data_402_python/assets/153448835/090d1304-6fff-47ad-aa26-79999d6c5ba3)
 ![output - index](https://github.com/SKaurGithub/data_402_python/assets/153448835/ac056cd2-1165-458e-a33b-4f1a20e32756)

    - As we can see, we were able to slice the string by indexing `[0:5]` which returned `Hello`
  - Strings are immutable, which means you can not change them. In order to store the changed string, you will need to store it in another variable
  - Built-In Function: `len()`
    - The len() function returns the length of a string

- Boolean & Equality Operators
  - Equality Operators: `==`, `!=`, `>`, `<`, `>=`, `<=`
    - These operators can help to compare values:
      ![Equality Operators](https://github.com/SKaurGithub/data_402_python/assets/153448835/398df4aa-e3c2-4b6c-853e-dd0d7c3f72f8)
      ![equality operators example](https://github.com/SKaurGithub/data_402_python/assets/153448835/23fdcc29-6b6c-4369-98d0-a2526b6d118f)
      ![equality operators output](https://github.com/SKaurGithub/data_402_python/assets/153448835/948846be-3827-47d4-bcaa-143f5e989945)



### Variables

- Variables Introduction
  - Variables are containers to store data, which can be referred back to
  - the assignment operator (=) as we are assigning a value/string
  - variable names need to be lower case
  - variable names should have underscores instead of spaces
  - they should have a descriptive name
  - Python Style Guide: [https://peps.python.org/pep-0008/](https://peps.python.org/pep-0008/)


### More on Strings

- Concatenation & Escape Characters
  - You can add strings to one another using the `+` operator (Please bear in mind that you cannot concatenate a string with a non-string using this method):<br>
    ![concat with plus](https://github.com/SKaurGithub/data_402_python/assets/153448835/1b3cc7f3-c237-4ce4-acac-ceb21014a152)
  - You can also use the f-string method:<br>
    ![f-string](https://github.com/SKaurGithub/data_402_python/assets/153448835/8b847c83-c72d-4b15-a91c-2e5d0d79a10b)
  - You can also use the format() method:<br>
    ![format()](https://github.com/SKaurGithub/data_402_python/assets/153448835/e8e58563-69f3-46cb-bf4d-51edb57d16cb)
  - The output will be the same for all 3 options:<br>
    ![output of concat](https://github.com/SKaurGithub/data_402_python/assets/153448835/32873843-8cb7-42b3-bdca-904bb7ae8f9c)


  - Python uses the backslash `\` as an escape character:
    - `\n` = Newline - inserts a new line
    - `\t` = Tab - inserts a tab
    - `\s` = inserts a space

- String Methods
  - There are different methods to manipulate strings such as:
    - .upper() = converts string to uppercase
    - .lower() = converts string to lowercase
    - .strip() = removes any whitespace from the start and the end of the string
    - .replace('oldText', 'newText') = replaces any occurrences of 'oldText' with 'newText' 
  - Further Python String Methods: [https://docs.python.org/3/library/stdtypes.html#string-methods](https://docs.python.org/3/library/stdtypes.html#string-methods)


### Control Flow

- This refers to the order in which the individual statements of a program are executed
- We use conditional statements for this, also called if-elif statements
- These are used to execute different blocks of code based on whether a certain condition is true or false.<br>
  ![conditional statement](Images/img.png)

### Collections

- Lists
  - A list allows you to create a list of values, which can be of any data type
  - They are index based, which means that each value can be found by its index
    ![list](img_1.png)
  
- Dictionaries
  - A dictionary is based on `{key: value}` pairs
  - Elements in dictionaries are access via keys
  - The key must be immutable (can be any data type other than a list or a dictionary) and unique
  - The value can be of any data type


### Loops

- While Loops
  - A while loop takes a code block and keeps executing it while a given condition stays `True`
  - The while statement repeats its action until this controlling condition becomes `False`
  - These statements need to be indented in the loop
  - A while loop starts with `while` followed by a boolean expression
  - It can run the risk of running forever if the condition never becomes `False`. This is called infinite loop.
  - To avoid an infinite loop, make sure your while loop condition eventually becomes `False` and that your loop is exited


- For Loop
  - A for loop is a counter-controlled loop, which means that the number of repetitions in a for loop is known a head of time
  - In each iteration (or repetition) of the for loop the code that is indented is repeated
  - A for loop starts with `for` followed by a variable that will hold each of the values of the sequence as we iterate through it


### Functions

- Functions allow us to write block of codes that break our code down into smaller modular parts
- They help our program to be more organised and makes our code reusable
- To create a function you need to start with `def` followed by the name of our function followed by parentheses
- Everything belonging to the functions needs to be indented:
  
- In order to execute a function, you will need to call the function:


