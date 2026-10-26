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
