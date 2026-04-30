# **MIT 6.100L – Lecture 3: Iteration (Loops)**

##  CORE IDEA

> Loops = repeat code until a condition or sequence ends
> Think of it as a machine that refuses to stop unless you *force logic into it*.

---

# 1. WHILE LOOPS (Condition-driven)

## Structure

```python
while <condition>:
    <code>
```

## How it works

* Check condition → True → run code
* Repeat
* Stop only when condition becomes False
* If never False → **infinite loop** 

## Reality check

If you don’t control the condition, your program becomes a prisoner.

---

## Example (Lost Forest)

```python
where = input("Go left or right? ")
while where == "right":
    where = input("Go left or right? ")
print("You got out!")
```

 Insight:

* Loop continues ONLY if input == "right"
* Any other input → escape 

---

## Counter Pattern (CRITICAL)

```python
n = int(input())
while n > 0:
    print('x')
    n = n - 1
```

 If you forget `n = n - 1` → infinite loop
This is where beginners silently fail.

---

## Infinite Loop Example

```python
while True:
    print("noooooo")
```

 Only stops by external force (CTRL+C) 

---

## Big Insight

> while loop = **uncertain repetition**

* You don’t know how many times it runs
* Depends on condition

---

# 2. FOR LOOPS (Sequence-driven)

## Structure

```python
for <var> in <sequence>:
    <code>
```

## How it works

* Takes values one by one from sequence
* Stops when sequence ends 

---

## Example

```python
for n in range(5):
    print(n)
```

Output:

```
0 1 2 3 4
```

---

## range()

```python
range(start, stop, step)
```

* start → default = 0
* stop → NOT included
* step → default = 1 

### Examples:

```python
range(5)        → 0,1,2,3,4
range(1,4)      → 1,2,3
range(1,4,2)    → 1,3
range(4,0,-1)   → 4,3,2,1
```

---

## Big Idea

> for loop = **controlled repetition**

* You KNOW how many times it runs

---

# 3. WHILE vs FOR (Don’t mix this up)

| Concept  | while                | for                |
| -------- | -------------------- | ------------------ |
| Control  | Condition            | Sequence           |
| End      | When condition False | When sequence ends |
| Risk     | Infinite loop        | Safe               |
| Use case | Unknown repetitions  | Known repetitions  |

---

#  4. COMMON PATTERNS

## Factorial

### while version

```python
i = 1
factorial = 1
while i <= x:
    factorial *= i
    i += 1
```

### for version

```python
factorial = 1
for i in range(1, x+1):
    factorial *= i
```

 Same logic, different control style 

---

## Running Sum

```python
mysum = 0
for i in range(10):
    mysum += i
```

Pattern:

* Initialize → `mysum = 0`
* Accumulate → `+=`

---

# 5. LOOPING MENTAL MODELS

## Pattern 1: Counter loop

* Track progress manually (while)

## Pattern 2: Sequence loop

* Let Python handle iteration (for)

## Pattern 3: Accumulator

* Build value over time (sum, factorial)

---

# 6. CRITICAL PITFALLS

*  Forgetting to update variable in while → infinite loop
*  Misunderstanding `range(stop)` → excludes stop
*  Case sensitivity in input ("right" ≠ "RIGHT") 
*  Thinking for loop can run forever → it cannot

---

# FINAL SUMMARY

* while → runs **while condition is True**
* for → runs **over a sequence**
* range → generates number sequences
* infinite loops happen when condition never changes
* loops rely on:

  * condition control (while)
  * sequence control (for)
* most problems = **counter + condition + update**

---

# One line proverb

> “A loop without control is a road without an exit.”

---

