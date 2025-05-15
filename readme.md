# Define the sorted and titled complete notes content

sorted_notes = """
📌 Python Basics

print() – Prints output to the screen.
Example:
print("Hello, world!")

input() – Reads input from the user.
Example:
name = input("Enter your name: ")

pass – Does nothing; used as a placeholder in a block of code.
Example:
if True:
    pass

end= in print – Changes what is printed at the end of a print statement (default is newline).
Example:
print("Hello", end="!") → prints "Hello!" without a new line after


🔤 String Methods

len() – Returns the number of items (like characters in a string).
Example:
len("apple") → 5

lower() – Changes all letters in a string to lowercase.
Example:
"HeLLo".lower() → "hello"

upper() – Converts all characters to uppercase.
Example:
"hello".upper() → "HELLO"

isalpha() – Checks if all characters in a string are only letters (no spaces, no numbers).
Example:
"abc".isalpha() → True

isdigit() – Checks if all characters in a string are digits.
Example:
"123".isdigit() → True

find() – Searches for part of a string and gives the index; returns -1 if not found.
Example:
"hello".find("e") → 1

index() – Like find(), but gives an error if the string is not found.
Example:
"hello".index("e") → 1

strip() – Removes whitespace from both ends of a string.
Example:
" hello ".strip() → "hello"

split() – Splits a string into a list using a separator (default is space).
Example:
"apple orange".split() → ['apple', 'orange']

join() – Joins elements of a list into a string using a separator.
Example:
"-".join(["a", "b", "c"]) → "a-b-c"

ljust() – Left-justifies a string in a field of a given width by padding with spaces.
Example:
"hi".ljust(5) → "hi   "

rjust() – Right-justifies a string in a field of a given width by padding with spaces.
Example:
"hi".rjust(5) → "   hi"

center() – Centers a string in a field of a given width by padding with spaces.
Example:
"hi".center(5) → " hi  "

.isupper() – Checks if all characters in the string are uppercase.
Example:
"HELLO".isupper() → True


🔁 Control Flow

if statement – Runs a block of code only if a condition is true.
Example:
age = 18
if age >= 18:
    print("You are an adult")

if elif – Handles multiple conditions in sequence.
Example:
x = 10
if x < 0:
    print("Negative")
elif x == 0:
    print("Zero")
else:
    print("Positive")

for loop – Repeats code for each item in a list or range.
Example:
for i in range(5):
    print(i)

while – Repeats code while a condition is true.
Example:
i = 0
while i < 5:
    print(i)
    i += 1


📦 Data Structures

list() – Creates a list.
Example:
list("abc") → ['a', 'b', 'c']

tuple – A data structure like a list, but immutable (cannot be changed).
Example:
my_tuple = (1, 2, 3)

dictionary and access of it – A collection of key-value pairs.
Example:
my_dict = {"name": "Alice"}
print(my_dict["name"]) → Alice

append() – Adds an item to the end of a list.
Example:
my_list.append(4)

insert() – Inserts an item at a specific index in a list.
Example:
my_list.insert(1, "new")

pop() – Removes and returns an item at a specific index (default is last).
Example:
my_list.pop()


🎲 Random & Security

import random – For pseudo-random number generation.
random.randint(1, 10) → Random number from 1 to 10

choice() – Returns a random item from a list.
Example:
random.choice([1, 2, 3])

import secrets – For secure random values (better for security).
secrets.choice([1, 2, 3]) → Secure random choice

import string – Provides string constants.
string.ascii_lowercase → 'abcdefghijklmnopqrstuvwxyz'
string.ascii_uppercase → 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'


🧠 Comprehensions & Lambdas

List comprehension – Compact way to create lists.
Example:
[i * 2 for i in range(5)] → [0, 2, 4, 6, 8]

With if/else:
[i if i % 2 == 0 else 0 for i in range(5)]

lambda function – Anonymous, one-line function.
Example:
add = lambda x, y: x + y
print(add(2, 3)) → 5


🧮 Built-in Functions

type() – Tells you the type of a value.
Example:
type(123) → <class 'int'>

abs() – Returns the absolute value of a number.
Example:
abs(-5) → 5

max() – Returns the largest value.
Example:
max(1, 5, 2) → 5

sum() – Adds all numbers in an iterable.
Example:
sum([1, 2, 3]) → 6

int() – Converts to an integer.
Example:
int("42") → 42

float() – Converts to a float.
Example:
float("3.14") → 3.14

range(start, stop, step) – Generates a sequence of numbers.
Example:
range(1, 5, 2) → 1, 3

square x**2 – Raises a number to a power (here, squaring).
Example:
x = 3
x**2 → 9


🔍 Regular Expressions (re)

import re – Used for working with regular expressions.

compile() – Compiles a regex pattern for reuse.
Example:
pattern = re.compile(r"\\d+")

search() – Searches for the first match of a pattern in a string.
Example:
re.search(r"cat", "concatenate")
Optional parameters:
- string (required): the text to search in.
- pos (optional): where to start searching.
- endpos (optional): where to stop searching.

findall() – Returns a list of all non-overlapping matches.
Example:
re.findall(r"\\d+", "There are 24 apples and 7 bananas") → ['24', '7']


📚 f-Strings & Formatting

f'string – Allows embedding variables in strings using {}.
Example:
name = "Alex"
print(f"Hello, {name}!") → Hello, Alex!

str.maketrans – Creates a mapping for string replacement.
Example:
table = str.maketrans("ae", "12")

.translate – Applies the mapping to a string.
Example:
"apple".translate(table) → "1ppl2"


🧪 Errors & Exceptions

raise ValueError() – Manually raises a ValueError exception.
Example:
raise ValueError("Invalid input")
"""

🌍 Global Variables

global – Allows a function to modify a variable defined outside of it.
