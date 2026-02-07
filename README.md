Fluent Programming Language
Fluent is a simple interpreted programming language designed to be easy to read, write, and learn.
It supports variables, conditionals, loops, functions, lists, strings, and built-in utilities, making it a great project for understanding language design and interpreters.

Documentation
This document describes the syntax, data types, operations, and features of the Fluent programming language.

Syntax Rules
# Single-line comments start with #

# Variables can be declared without any identifier keyword
# Every statement must end with a semicolon

a = 10;
b = "Fluent";

# Conditions do not require parentheses
if 1 == 1 {
  pass; # Blocks with curly braces cannot be empty
}

# Boolean values
c = true; # true = 1, false = 0
print(c); # Output: 1


Data Types & Keywords
Supported Data Types

Fluent supports the following data types:

Boolean
String
Number
List


# Boolean
boolVar = true;

# String
stringVar = "Fluent";

# Number
numVar = 10;

# List (can hold mixed types)
list = [1, 2.2, true, "Hello"];

Keywords
["and", "or", "not", "if", "else", "while", "for", "step",
 "until", "continue", "break", "func", "return", "pass"]

String Operations
# Concatenate strings
str1 = "Hello, " + "World";
print(str1); # Hello, World

# Access character by index
char = str1[2];
print(char); # l

# Repeat string
str2 = str1[2] * 5;
print(str2); # lllll

# Add number to string
str3 = str2 + 5;
print(str3); # lllll5

List Operations
# Add element to list
list1 = [1, 2.2, true, "Hello"] + 100;
print(list1); # [1, 2.2, 1, "Hello", 100]

# Remove element at index
list2 = list1 - 1;
print(list2); # [1, 1, "Hello", 100]

# Access element at index
value = list2[2];
print(value); # Hello

# Concatenate two lists
list3 = [1, 2] * [100, 200];
print(list3); # [1, 2, 100, 200]


Conditionals
Fluent supports if–else if–else conditional branching.
a = 5;
b = 7;

if a == b {
  print("Condition 1 is true");
} else if false {
  print("Condition 2 is true");
} else if a != b and a == 5 {
  print("Condition 3 is true");
} else {
  pass;
}

# Output:
# Condition 3 is true


Functions
func add(num1, num2) {
  print("Add Function");
  return num1 + num2;
}

Functions can be assigned to variables:
c = add(1, 2);
print("c = " + c); # c = 3
a = add;
print(a(3, 4));
# Add Function
# 7

Arrow Functions (Single-Line)
func oopify(x) => x + "oop";
print(oopify("Hello")); # Hellooop

Loops
While Loop

a = 1;
while a <= 5 {
  print(a);
  a = a + 1;
}

Output
1
2
3
4
5

For Loop
for i = 0 until 5 {
  print(i);
}

Output
0
1
2
3
4

For Loop with Step
for i = 0 until 4 step 2 {
  print(i);
}

Output
0
2


Built-In Functions

# Print
print("Hello, world!");

# PrintReturn
str = printReturn("Hello, world!");

# Input
userInput = input();

# Type checks
list = [1, 2];
isLis = isList(list);
isNum = isNumber(42);

f = func () {
  pass;
}
isFunc = isFunction(f);

isStr = isString("Fluent");

# Length
length = len(list);
length = len("Fluent");

# Absolute value
num = abs(-123);

Why Fluent?
Fluent is designed to:

  Be simple and readable

  Demonstrate interpreter and language design concepts

  Help beginners understand how real languages work internally
