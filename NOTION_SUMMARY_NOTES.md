# #DAY 24 — LISTS IN PYTHON

---

## 1. Introduction to Lists

A **list** is a collection of multiple values stored in a single variable.

Lists are:

- Ordered
- Mutable (can be changed)
- Allow duplicate values

Real-world idea:

- A list of students
- A list of marks
- A shopping list

---

## 2. Creating a List

Lists are created using square brackets `[ ]`.

```python
fruits= ["apple","banana","mango"]x
print(fruits)
```

---

## 3. List with Different Data Types

A list can store different types of values.

```python
data= ["Devansh",21,True]
print(data)
```

---

## 4. Accessing Elements (Indexing)

```python
fruits= ["apple","banana","mango"]

print(fruits[0])
print(fruits[1])
```

---

## 5. Negative Indexing

```python
print(fruits[-1])
```

Accesses elements from the end.

---

## 6. Changing List Elements

Lists are mutable, so values can be changed.

```python
fruits= ["apple","banana","mango"]

fruits[1]="orange"
print(fruits)
```

---

## 7. Adding Elements

### `append()` — Add at end

```python
fruits.append("grapes")
```

---

### `insert()` — Add at specific position

```python
fruits.insert(1,"kiwi")
```

---

## 8. Removing Elements

### `remove()` — Remove by value

```python
fruits.remove("banana")
```

---

### `pop()` — Remove by index

```python
fruits.pop(1)
```

## 9. On-the-Go List Creation (List Comprehension)

Sometimes we want to **create a list quickly in one line** instead of using loops.

This is called **list comprehension**.

### Basic Syntax

```python
new_list= [expression for item in iterable]
```

---

### Example 1 — Simple Numbers

```python
nums= [i for i in range(5)]
print(nums)
```

Output:

```python
[0, 1, 2, 3, 4]
```

---

### Example 2 — Squares of Numbers

```python
squares= [i*i for i in range(1,6)]
print(squares)
```

Output:

```python
[1, 4, 9, 16, 25]
```

---

### Example 3 — With Condition

```python
even_nums= [i for i in range(10) if i%2==0]
print(even_nums)
```

Output:

```python
[0, 2, 4, 6, 8]
```

## 10. Important Points

- Lists are ordered collections
- Lists are mutable
- Can store multiple data types
- Support indexing and looping

---

# 📝 SUMMARY — LISTS

- Created using `[ ]`
- Store multiple values
- Mutable (can change)
- Supports indexing and loops

---

## One-Line Concept

> A list is a mutable collection used to store multiple values in a single variable.
> 

# #DAY 25 — LIST METHODS IN PYTHON

---

## 1. Introduction to List Methods

**List methods** are built-in functions used to perform operations on lists.

They help us:

- Add elements
- Remove elements
- Sort data
- Modify lists easily

They are used like:

```python
list_name.method()
```

---

## 2. `append()` — Add Element at End

```python
fruits= ["apple","banana"]
fruits.append("mango")
print(fruits)
```

Output:

```python
['apple', 'banana', 'mango']
```

---

## 3. `insert()` — Add at Specific Position

```python
fruits= ["apple","banana"]
fruits.insert(1,"orange")
print(fruits)
```

---

## 4. `remove()` — Remove by Value

```python
fruits= ["apple","banana","mango"]
fruits.remove("banana")
print(fruits)
```

---

## 5. `pop()` — Remove by Index

```python
fruits= ["apple","banana","mango"]
fruits.pop(1)
print(fruits)
```

---

## 6. `clear()` — Remove All Elements

```python
fruits= ["apple","banana"]
fruits.clear()
print(fruits)
```

Output:

```
[]
```

---

## 7. `index()` — Find Position

```python
fruits= ["apple","banana","mango"]
print(fruits.index("banana"))
```

---

## 8. `count()` — Count Occurrences

```python
nums= [1,2,2,3]
print(nums.count(2))
```

---

## 9. `sort()` — Sort List

```python
nums= [5,2,9,1]
nums.sort()
print(nums)
```

---

### Reverse Sorting

```python
nums.sort(reverse=True)
```

---

## 10. `reverse()` — Reverse List

```python
nums= [1,2,3]
nums.reverse()
print(nums)
```

---

## 11. `copy()` — Copy List

```python
a= [1,2,3]
b=a.copy()
print(b)
```

---

## 12. `extend()` — Add Multiple Elements

```python
a= [1,2]
b= [3,4]
a.extend(b)
print(a)
```

---

# 📝 SUMMARY — LIST METHODS

- `append()` → add at end
- `insert()` → add at position
- `remove()` → remove by value
- `pop()` → remove by index
- `clear()` → remove all
- `index()` → find position
- `count()` → count values
- `sort()` → sort list
- `reverse()` → reverse list
- `copy()` → duplicate list
- `extend()` → add multiple items

---

## One-Line Concept

> List methods are built-in functions that help modify, organize, and manage list data efficiently.
> 

---

# #DAY 26 — TUPLES IN PYTHON

---

## 1. Introduction to Tuples

A **tuple** is a collection of multiple values stored in a single variable, similar to a list.

👉 **Tuples are immutable (cannot be changed)**

Tuples are:

- Ordered
- Immutable
- Allow duplicate values

---

## 2. Creating a Tuple

```python
numbers= (1,2,3)
print(numbers)
```

---

## 3. Single Element Tuple

```python
t= (5,)
print(t)
```

Without comma:

```python
t= (5)# Not a tuple
```

---

## 4. Accessing Elements (Indexing)

```python
nums= (10,20,30)

print(nums[0])
print(nums[1])
```

---

## 5. Negative Indexing

```python
print(nums[-1])
```

---

## 6. Tuple Slicing

Slicing allows us to extract a part of a tuple.

### Syntax

```python
tuple[start:end]
```

---

### Example

```python
nums= (10,20,30,40,50)

print(nums[1:4])
```

Output:

```python
(20, 30, 40)
```

---

### More Examples

```python
print(nums[:3])# From start
print(nums[2:])# Till end
print(nums[:])# Full tuple
```

---

## 7. Immutability of Tuples

```python
nums= (1,2,3)

# nums[0] = 10  ❌ Error
```

👉 Elements cannot be changed after creation.

---

## 8. Looping Through Tuple

```python
nums= (1,2,3)

for n in nums:
print(n)
```

---

## 9. Why Use Tuples?

- When data should not change
- Faster than lists
- Used for fixed values

Example:

```python
coordinates= (10,20)
```

---

## 11. Tuple vs List

| Feature | List | Tuple |
| --- | --- | --- |
| Brackets | `[ ]` | `( )` |
| Mutable | ✔ Yes | ❌ No |
| Methods | Many | Few |
| Speed | Slower | Faster |

---

# 📝 SUMMARY — TUPLES

- Created using `( )`
- Immutable
- Supports indexing and slicing
- Used for fixed data

---

## One-Line Concept

> A tuple is an immutable collection that supports indexing and slicing but does not allow modification.
> 

# #DAY 27 — TUPLE METHODS IN PYTHON

---

## 1. Introduction to Tuple Methods

Unlike lists, tuples are **immutable**, so they have **very few methods**.

👉 Only two main built-in methods are available:

- `count()`
- `index()`

---

## 2. `count()` — Count Occurrences

```python
nums= (1,2,2,3,2)
print(nums.count(2))
```

---

## 3. `index()` — Find Position

```python
nums= (10,20,30,20)
print(nums.index(20))
```

👉 Returns index of **first occurrence**

---

## 4. Modifying Tuple (Using List Conversion)

Since tuples are immutable, we **cannot change them directly**.

But we can convert them into a list, modify, and convert back.

### Example

```python
nums= (1,2,3)

temp=list(nums)# convert to list
temp[1]=100# modify
nums=tuple(temp)# convert back to tuple

print(nums)
```

Output:

```python
(1, 100, 3)
```

---

## 5. Concatenating Tuples

We can combine two tuples using `+`.

### Example

```python
t1= (1,2)
t2= (3,4)

result=t1+t2
print(result)
```

Output:

```python
(1, 2, 3, 4)
```

---

## 6. Extra Operations

### Length

```python
nums= (1,2,3)
print(len(nums))
```

---

### Membership Check

```python
print(2 in nums)
```

---

### Looping

```python
for n in nums:
print(n)
```

---

# 📝 SUMMARY — TUPLE METHODS

- `count()` → counts occurrences
- `index()` → finds position
- `len()` → gives the length
- Convert to list → modify → convert back
- Tuples can be concatenated using `+`

---

## One-Line Concept

> Tuples are immutable, but we can modify them by converting to list and can combine them using concatenation.
> 

# #DAY 28 — EXERCISE 3: KBC

## Kaun Banega Crorepati (KBC) — Python Game

---

## 🎯 Problem Statement

Create a simple **KBC-style quiz game** in Python where:

- Questions are asked one by one
- Each question has 4 options
- User enters their answer
- If correct → move to next question
- If wrong → game ends
- Show total winnings at the end

# #DAY 30 — f-strings IN PYTHON

---

## 1. Introduction to f-strings

**f-strings (formatted strings)** are used to insert variables directly inside strings.

They make string formatting **easy, readable, and fast**.

---

## 2. Basic Syntax

```python
f"string{variable}"
```

👉 Add `f` before the string

👉 Use `{ }` to insert variables

---

## 3. Simple Example

```python
name="Devansh"
country="India"

print(f"My name is{name} and I am from {country}.")
```

Output:

```python
My name is Devansh and I am 21 years old.
```

---

## 4. Using Expressions Inside F-Strings

We can also perform calculations inside `{ }`.

```python
a=5
b=3

print(f"Sum is{a+b}")
```

Output:

```python
Sum is 8
```

---

## 5. Using Functions Inside F-Strings

```python
name="devansh"

print(f"Uppercase:{name.upper()}")
```

---

## 6. Formatting Numbers

```python
price=99.4567

print(f"Price:{price:.2f}")
```

Output:

```python
Price: 99.46
```

👉 `:.2f` → 2 decimal places

---

## 7. Multiline F-Strings

```python
name="Rahul"
age=20

print(f"""
Name:{name}
Age:{age}
""")
```

---

## 8. Why Use F-Strings?

- Cleaner than `+` concatenation
- Faster and more readable
- Supports expressions

---

## 9. Old Method (For Comparison)

```python
name="Rahul"
age=20

print("My name is",name,"and age is",age)
```

👉 Less clean compared to f-strings

---

# 📝 SUMMARY — F-STRINGS

- Use `f` before string
- Insert variables using `{}`
- Can include expressions and functions
- Makes code clean and readable

---

## One-Line Concept

> F-strings allow embedding variables and expressions directly inside strings using `{}`.
> 

# #DAY 31 — DOCSTRINGS & PEP 8

---

## 1. Introduction

Writing code is not just about making it work — it should also be **easy to read and understand**.

Python strongly focuses on **clean and readable code**, which is guided by:

- **Docstrings** → Explain what the code does
- **PEP 8** → Rules for writing clean code
- **Zen of Python** → Philosophy behind these rules

---

# 🧠 PART 1 — DOCSTRINGS

---

## 2. What are Docstrings?

A **docstring** is a string used to describe a function, module, or class.

It is written using triple quotes `""" """`.

---

## 3. Example

```python
def add(a,b):
	"""takes in two numbers and return the sum of two numbers"""
	return a+b
```

---

## 4. Accessing Docstring

```python
print(add.__doc__)
```

---

## 5. Why Use Docstrings?

- Explain purpose of function
- Improve readability
- Help other developers
- Used in documentation tools

---

# 🧠 PART 2 — PEP 8 & ZEN OF PYTHON

---

## 6. What is PEP 8?

**PEP 8** is the official style guide for Python.

👉 It tells us **how to write clean, readable, and consistent code**

But the question is:

👉 *Why should we follow PEP 8?*

The answer lies in the **Zen of Python**.

---

## 7. Zen of Python (by Tim Peters)

Run this in Python:

```python
import this
```

### Key Lines from Zen

- **Beautiful is better than ugly**
- **Simple is better than complex**
- **Readability counts**
- **Explicit is better than implicit**
- **There should be one obvious way to do it**

---

## 8. Connecting Zen → PEP 8

PEP 8 is basically the **practical implementation of the Zen of Python**.

Let’s connect them:

---

### 🔹 “Readability counts”

👉 PEP 8 says:

```python
# Good
def add(a,b):
	return a+b
```

```python
# Bad
def add(a,b):return a+b
```

---

### 🔹 “Simple is better than complex”

👉 Avoid messy code

```python
# Good
total= a + b 
```

---

### 🔹 “Explicit is better than implicit”

👉 Use clear variable names

```python
# Good
student_marks=90
```

```python
# Bad
sm=90
```

---

### 🔹 “Beautiful is better than ugly”

👉 Proper spacing, formatting, indentation

```python
a= 5 + 3 ✔
```

---

## 9. Important PEP 8 Rules

### ✔ Indentation

Use 4 spaces

```python
if True:
	print("Hello")
```

---

### ✔ Naming (snake_case)

```python
user_name="Devansh"
```

---

### ✔ Spacing

```python
a= 5 + 3 
```

---

### ✔ Line Length

Keep lines under 79 characters

---

### ✔ Blank Lines

Separate functions clearly

---

# 🧠 FINAL UNDERSTANDING

- **Zen of Python** → Philosophy (Why clean code matters)
- **PEP 8** → Rules (How to write clean code)
- **Docstrings** → Explanation (What the code does)

---

# 📝 SUMMARY

- Docstrings describe code
- PEP 8 improves readability
- Zen of Python explains why readability matters
- Clean code = easy to read + easy to maintain

---

## One-Line Concept

> The Zen of Python gives the philosophy, PEP 8 gives the rules, and docstrings give the explanation — together they make Python code clean and readable.
> 

# #DAY 32 — RECURSION IN PYTHON

---

## 1. Introduction to Recursion

**Recursion** is a process where a function **calls itself** to solve a problem.

Instead of using loops, recursion breaks a problem into **smaller subproblems**.

---

## 2. Basic Idea

👉 A function keeps calling itself until a condition is met.

That condition is called the **base case**.

---

## 3. Basic Syntax

```
deffunction_name():
ifcondition:
returnvalue# base case
else:
returnfunction_name()# recursive call
```

---

## 4. Example — Countdown

```python
def countdown(n):
	if n==0:
		print("Done")
	else:
		print(n)
		countdown(n-1)

countdown(5)
```

Output:

```python
5
4
3
2
1
Done
```

---

## 5. Important Concept

Every recursive function must have:

### ✔ Base Case

Stops the recursion

### ✔ Recursive Case

Function calling itself

---

## 6. Example — Factorial

```python
def factorial(n):
	if n==0:
		return 1
	else:
		return n*factorial(n-1)

print(factorial(5))
```

Output:

```python
120
```

---

## 7. How Recursion Works (Step-by-Step)

For `factorial(3)`:

```python
3 * factorial(2)
2 * factorial(1)
1 * factorial(0)
```

Then:

```python
1 * 1 = 1
2 * 1 = 2
3 * 2 = 6
```

---

## 8. Recursion vs Loop

| Feature | Recursion | Loop |
| --- | --- | --- |
| Uses function calls | ✔ Yes | ❌ No |
| Uses memory | More | Less |
| Easy for some problems | ✔ Yes | ❌ Sometimes |

---

## 9. Important Points

- Must have a base case
- Otherwise → infinite recursion
- Uses function call stack
- Useful for problems like factorial, tree traversal

---

## 10. Common Mistake

```python
def func(n):
	return func(n-1)# ❌ No base case
```

👉 This will cause **infinite recursion error**

---

# 📝 SUMMARY — RECURSION

- Function calling itself
- Needs base case + recursive case
- Breaks problem into smaller parts

---

## One-Line Concept

> Recursion is a technique where a function solves a problem by calling itself until a base condition is met.
> 

# #DAY 33 — SETS IN PYTHON

---

## 1. Introduction to Sets

A **set** is a collection of **unique elements**.

👉 Sets do **not allow duplicate values**

👉 Sets are **unordered** (no fixed position/index)

Real-world idea:

- A group of unique students
- Unique phone numbers
- Unique IDs

---

## 2. Creating a Set

Sets are created using `{ }`.

```python
nums= {1,2,3,4}
print(nums)
```

---

## 3. Duplicate Values Removed Automatically

```python
nums= {1,2,2,3}
print(nums)
```

Output:

```python
{1, 2, 3}
```

---

## 4. Unordered Nature

```python
nums= {5,1,3}
print(nums)
```

👉 Output order may change

---

## 5. Set Operations

### Union (Combine sets)

```python
a= {1,2}
b= {3,4}

print(a|b)
```

---

### Intersection (Common elements)

```python
print(a&b)
```

---

### Difference

```python
print(a-b)
```

---

## 6. Looping Through Set

```python
for i in nums:
	print(i)
```

---

## 7. Important Points

- No duplicate values
- Unordered → no indexing
- Mutable (can add/remove)
- Used for unique data

---

## 8. Empty Set Warning

```python
a= {}# ❌ This is a dictionary
```

Correct way:

```python
a=set()
```

---

# 📝 SUMMARY — SETS

- Store unique values
- Created using `{ }`
- No duplicates allowed
- No indexing
- Useful for set operations

---

## One-Line Concept

> A set is an unordered collection of unique elements used to remove duplicates and perform mathematical set operations.
> 

# #DAY 34 — SET METHODS IN PYTHON

---

## 1. Introduction to Set Methods

Set methods are used to **modify sets and perform operations** on them.

👉 Sets are mainly used for **unique data and mathematical operations**

---

## 2. `add()` — Add Element

```python
s= {1,2}
s.add(3)
print(s)
```

---

## 3. `update()` — Add Multiple Elements

```python
s= {1,2}
s.update([3,4])
print(s)
```

---

## 4. `remove()` — Remove Element

```python
s= {1,2,3}
s.remove(2)
```

👉 Error if element not found

---

## 5. `discard()` — Safe Remove

```python
s.discard(10)
```

👉 No error if element is absent

---

## 6. `pop()` — Remove Random Element

```python
s= {1,2,3}
s.pop()
```

👉 Removes random item

---

## 7. `clear()` — Remove All Elements

```python
s.clear()
```

---

## 8. `union()` — Combine Sets

```python
a= {1,2}
b= {3,4}

print(a.union(b))
```

---

## 9. `intersection()` — Common Elements

```python
a= {1,2,3}
b= {2,3,4}

print(a.intersection(b))
```

---

## 10. `difference()` — Unique Elements

```python
print(a.difference(b))
```

---

## 11. `symmetric_difference()` — Non-common Elements

```python
print(a.symmetric_difference(b))
```

---

## 12. `issubset()` — Check Subset

```python
a= {1,2}
b= {1,2,3}

print(a.issubset(b))
```

---

## 13. `issuperset()` — Check Superset

```python
print(b.issuperset(a))
```

---

## 14. `isdisjoint()` — No Common Elements

```python
a= {1,2}
b= {3,4}

print(a.isdisjoint(b))
```

---

# 📝 SUMMARY — SET METHODS

- `add()` → add element
- `update()` → add multiple
- `remove()` / `discard()` → remove
- `pop()` → remove random
- `clear()` → empty set
- `union()` → combine sets
- `intersection()` → common values
- `difference()` → unique values
- `symmetric_difference()` → non-common
- `issubset()` / `issuperset()` → relation
- `isdisjoint()` → no common elements

---

## One-Line Concept

> Set methods help manage unique data and perform mathematical operations like union, intersection, and difference.
> 

#DAY 35 — DICTIONARIES IN PYTHON

🟣 Holy Hackathon — Python Turtle Projects

To Do List
