=========================================================================================================================================


# Python 

Python is a high-level, interpreted, interactive and object-oriented **scripting language**. Python is designed to be highly readable.

1. Python is *Interpreted* − Python is processed at runtime by the interpreter. You do not need to compile your program before executing it. This is similar to PERL and PHP.

2. Python is *Interactive* − You can actually sit at a Python prompt and interact with the interpreter directly to write your programs.

3. Python is *Object-Oriented* − Python supports Object-Oriented style or technique of programming that encapsulates code within objects.




=========================================================================================================================================


### Interactive Interpreter
You can start Python from Unix, DOS, or any other system that provides you a command-line interpreter or shell window. (In VSCode click on "Terminal" > "New Terminal")

Enter **python** the command line.

Start coding right away in the interactive interpreter!!




=========================================================================================================================================


### Our first python command

Each line in python is python command. Each command consists of special **keywords** that PYthon recognizes. Keywords are reserved words that cannot be used as variable names. 

For example, in the following code, we use the keyword `print` to print the string `Hello World!` to the screen. Type the following text at the Python prompt and press the Enter −

```
print('Hello world')
```



=========================================================================================================================================


### Python Identifiers

A Python identifier is a name used to identify a **variable, function, class, module** or other **object**. An identifier starts with a letter A to Z or a to z or an underscore (_) followed by zero or more letters, underscores and digits (0 to 9). It is *case-senstive* !!

A python **variable** is a name that refers to a value. Variables are created when they are first assigned values using the = operator. A variable can be assigned a value of any type, and that type can change as the program runs.

```
Apple = 5
apple = 10
print(Apple)
print(apple)
```


=========================================================================================================================================


### Lines and Indentation

Blocks of code are denoted by line indentation, which is rigidly enforced.

The number of spaces in the indentation is variable, but all statements within the block must be indented the same amount. For example −

```
if True:
   print "True"
else:
   print "False"
```


Statements in Python typically end with a new line. Python does, however, allow the use of the line continuation character (\) to denote that the line should continue. For example −

```
total = item_one + \
        item_two + \
        item_three
```


=========================================================================================================================================


### Quotation in Python

Python accepts single ('), double (") and triple (''' or """) quotes to denote string literals, as long as the same type of quote starts and ends the string.

The triple quotes are used to span the string across multiple lines. For example, all the following are legal −

```
word = 'word'
sentence = "This is a sentence."
paragraph = """This is a paragraph. It is
made up of multiple lines and sentences."""
```



=========================================================================================================================================


### Comments in Python

A hash sign (#) that is not inside a string literal begins a comment. 

```
# First comment
print "Hello, Python!" # second comment
```



=========================================================================================================================================


### Assigning Values to Variables

The equal sign (=) is used to assign values to variables.

The operand to the left of the = operator is the name of the variable and the operand to the right of the = operator is the value stored in the variable. For example −

```
counter = 100          # An integer assignment
miles   = 1000.0       # A floating point
name    = "John"       # A string

print(counter)
print(miles)
print(name)
```



=========================================================================================================================================


### Python scripts

A Python script is just a plain text file, and the convention is to use the extension .py (instead of e.g. .txt) to let programs know that it holds Python code.

We’re going to name our first script file **exercise_hello_world.py** by saving the code below in Tutorial_0 folder.

```
counter = 100          # An integer assignment
miles   = 1000.0       # A floating point
name    = "John"       # A string

print(counter)
print(miles)
print(name)
```

We can now type

```
python exercise_hello_world.py
```

to get Python to run our script file.

Now, LET'S JUMP TO THE JUPYTER NOTEBOOK.

=========================================================================================================================================


### Standard Data Types
The data stored in memory can be of many types. For example, a person's age is stored as a numeric value and his or her address is stored as alphanumeric characters. Python has various standard data types that are used to define the operations possible on them and the storage method for each of them.

Python has five standard data types −

* Numbers
* String
* List
* Tuple
* Dictionary


```
# Python numbers
# Numeric values
foo = 5

# Python strings
# Contiguous set of characters
bar_1 = 'Hello World!'
bar_2 = "Hello World!" #both are assigned similar values

# Python lists
# Ordered sequence of values
baz = [1, 2, 3, 4, 5]

# Python tuples
# Ordered sequence of values. Similar to lists but immutable (modifications not allowed)
qux = (1, 2, 3, 4, 5)
#try to modify qux
qux[0] = 10 #this will throw an error

# Python dictionaries
# Unordered key-value pairs
quux = {'foo': 1, 'bar': 2, 'baz': 3}
```



=========================================================================================================================================


### Lists and Tuples

A list contains items separated by commas and enclosed within square brackets ([]). To some extent, lists are similar to arrays in C. One difference between them is that all the items belonging to a list can be of different data type.

```
list = [ 'abcd', 786 , 2.23, 'john', 70.2 ]
tinylist = [123, 'john']

print(list)          # Prints complete list
print(list[0])       # Prints first element of the list
print(list + tinylist) # Prints concatenated lists
```


Lists are enclosed in brackets ( [ ] ) and their elements and size can be changed, while tuples are enclosed in parentheses ( ( ) ) and cannot be updated. Tuples can be thought of as read-only lists. For example −

```
tuple = ( 'abcd', 786 , 2.23, 'john', 70.2  )
tinytuple = (123, 'john')

print(tuple)               # Prints the complete tuple
print(tuple[0])            # Prints first element of the tuple. These are zero indexed
print(tuple[1])            # Prints second element of the tuple. 
print(tuple[2])            # Prints third element of the tuple.
print(tuple[1:])           # Prints elements starting from 2nd till last element
print(tuple[1:3])          # Prints elements of the tuple starting from 2nd till 3rd
print(tuple + tinytuple)   # Prints concatenated tuples
```

Here is how indexing works in Python for a string called "foobar" −
+---+---+---+---+---+---+
| F | o | o | b | a | r |
+---+---+---+---+---+---+
0   1   2   3   4   5   6
6  -5  -4  -3  -2  -1



=========================================================================================================================================


### Dictionary

Python's dictionaries are kind of hash table type. 
Python dictionaries are a mapping of key-value pairs. This means each element in the dictionary is accessed using its key. For example −

```
dict = {}
dict['one'] = "This is one"
dict[2]     = "This is two"

tinydict = {'name': 'john','code':6734, 'dept': 'sales'}
print(dict['one'])          # Prints value for 'one' key
print(dict[2])              # Prints value for 2 key
print(tinydict)             # Prints complete dictionary
print(tinydict['code'])     # Prints value for 'code' key 
```



=========================================================================================================================================


### Operators

Python language supports the following types of operators - 

* Arithmetic Operators
* Comparison (Relational) Operators
* Assignment Operators
* Logical Operators
* Bitwise Operators
* Membership Operators
* Identity Operators


Let us see what some of them look like:



Arithmetic operators - 


+ Addition	Adds values on either side of the operator.	a + b = 30
- Subtraction	Subtracts right hand operand from left hand operand.	a – b = -10
* Multiplication	Multiplies values on either side of the operator	a * b = 200
/ Division	Divides left hand operand by right hand operand	b / a = 2
% Modulus	Divides left hand operand by right hand operand and returns remainder	b % a = 0
** Exponent	Performs exponential (power) calculation on operators	a**b =10 to the power 20



Comparision operators -


==	If the values of two operands are equal, then the condition becomes true.	(a == b) is not true.
!=	If values of two operands are not equal, then condition becomes true.	(a != b) is true.
>	If the value of left operand is greater than the value of right operand, then condition becomes true.	(a > b) is not true.
<	If the value of left operand is less than the value of right operand, then condition becomes true.	(a < b) is true.
>=	If the value of left operand is greater than or equal to the value of right operand, then condition becomes true.	(a >= b) is not true.
<=	If the value of left operand is less than or equal to the value of right operand, then condition becomes true.	(a <= b) is true.


Assignment Operators - 


=	Assigns values from right side operands to left side operand	c = a + b assigns value of a + b into c
+= Add AND	It adds right operand to the left operand and assign the result to left operand	c += a is equivalent to c = c + a
-= Subtract AND	It subtracts right operand from the left operand and assign the result to left operand	c -= a is equivalent to c = c - a
*= Multiply AND	It multiplies right operand with the left operand and assign the result to left operand	c *= a is equivalent to c = c * a
/= Divide AND	It divides left operand with the right operand and assign the result to left operand	c /= a is equivalent to c = c / a


Logical Operators - 


[and Logical AND]	If both the operands are true then condition becomes true.	(a and b) is true.
[or Logical OR]	If any of the two operands are non-zero then condition becomes true.	(a or b) is true.
[not Logical NOT]	Used to reverse the logical state of its operand.	Not(a and b) is false.

Boolean variables
What are boolean variables? They are variables that can take only two values: True or False.
Boolean variables are used to store the truth value of an expression. For example, the expression 1 < 2 is True, while the expression 1 > 2 is False.
Boolean variables are very useful in programming. They are often used as flags to indicate whether certain conditions have been met. For example, you can have a boolean variable called is_logged_in to indicate whether a user has logged in to a website or not.

Boolean operators
Boolean operators are operators that are used to perform logical operations on boolean variables. The three basic boolean operators are: and, or, and not.