# My Lecture 3 Notes (Iteration)


# OSSU - Lecture 3: Iteration (Loops)

## What is Iteration?
Iteration = repeating a block of code multiple times.

 Used when you want to repeat tasks, Process multiple values,Avoid writing same code again.

---

# While Loop

## Structure

while condition:
    # code runs


## How it works

* Check condition
* If True → run code
* Repeat
* Stop when condition becomes False

---

## Example

n = 3

while n > 0:
    print(n)
    n = n - 1


Output:

3
2
1


---

## Infinite Loop 

while True:
    print("hello")


This never stops!

---

## Key Idea

* You must change something inside loop
* Otherwise → infinite loop

---

# Counter

Use variable to track loop:

count = 0

while count < 5:
    print(count)
    count += 1


---

# Example: Factorial (important)

x = 4
i = 1
factorial = 1

while i <= x:
    factorial *= i
    i += 1

print(factorial)

---

# For Loop (simple loop)

## Structure

for variable in sequence:
    # code

---

##  Example

for i in range(5):
    print(i)

Output:

0 1 2 3 4

---

# range()

Generates sequence of numbers:

range(start, stop, step)


Example:

range(5)        # 0,1,2,3,4
range(1,5)      # 1,2,3,4
range(1,10,2)   # 1,3,5,7,9

---

# While vs For

 While Loop                                       For Loop            
 ----------------------------                    -------------------
 Runs while condition is True                   - Runs for a sequence 
 Risk of infinite loop                          - Safer               
 More control                                   - Simpler             

---

# Sum Example

mysum = 0

for i in range(10):
    mysum += i

print(mysum)


 Adds numbers from 0 to 9

---

#  Key Concepts

* Loops repeat code
* while = condition-based loop
* for = sequence-based loop
* range() generates numbers
* Always avoid infinite loops

---

# Debugging Tip

* Write small code
* Test often
* Fix errors early

 Don’t write big program at once

---

# 🪞 Reflection (write yourself)

* What was easy: all of it is easy to understand.
* What was confusing:range is a little bit confusing for me but in java for loop is more easier to use i think?
* What program can I build with loops:now i can improve my guessgame with while loop to track my state.

````
