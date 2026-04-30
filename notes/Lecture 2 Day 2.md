# 📚 My Lecture 2 Notes

# OSSU - Lecture 2: Strings, Input/Output, and Branching

## Recap from Lecture 1
- Variables store values
- Expressions evaluate to a value
- Programs run line by line
- Good naming and comments are important

---

## Strings (str)

A string is a sequence of characters:
- letters, numbers, spaces, symbols

Example:

a = "hello"
b = 'world'


###  String Operations

* Concatenation (join):

a + b   # "helloworld"


* Repeat:


a * 3   # "hellohellohello"

---

## String Length

Use `len()`:

s = "abc"
len(s)  # 3

---

## Indexing (access characters)

s = "abc"

s[0]  # "a"
s[1]  # "b"
s[-1] # "c"

 Index starts at **0**

---

## Slicing (substring)

s = "abcdefgh"

s[3:6]    # "def"
s[:3]     # "abc"
s[::-1]   # reverse string

Format:

[start : stop : step]


---

## Immutable Strings

Strings cannot be changed:

s = "car"
s[0] = "b"   # ❌ error

But you can create a new string:

s = "b" + s[1:]

---

## Output (print)

print("Hello")
print(3 + 2)  # 5

Multiple values:

print("I have", 3, "apples")

---

## Input

name = input("Enter your name: ")

Important:

* `input()` ALWAYS returns a **string**

---

### Convert input to number

num = int(input("Enter number: "))

---

## Example Problem

text = input("Type anything: ")
print(5 * text)

If input = "hi" → output:

hihihihihi

---

## F-Strings (formatted output)

name = "Sam"
age = 18

print(f"My name is {name} and I am {age}")

---

## Branching (Decision Making)

Programs can choose what to do:

if condition:
    # do this
else:
    # do something else
    
---

## Comparison Operators

x > y
x < y
x == y
x != y

 Result is **True or False (Boolean)**

---
## Logical Operators

a and b
a or b
not a

---

## If / Elif / Else

if x > y:
    print("x is bigger")
elif x == y:
    print("equal")
else:
    print("y is bigger")

Note: Only ONE block runs

---

## ⚠️ Indentation (VERY IMPORTANT)

Python uses indentation to define blocks:

if x > 0:
    print("positive")  # must be indented

---

## Key Concepts

* Strings are sequences of characters
* Input is always string → convert if needed
* Programs make decisions using conditions
* Indentation controls program structure

---

## Reflection (write yourself)

* What was easy: most of it are easy cus i have already know it from java i can grasp the concept
* What was confusing: slicing is a bit annoying to understand but still i understand it now.
* What will I build with this: i will build a simple guessing game using if else if i have learned so you can check it in my projects folder.

````

