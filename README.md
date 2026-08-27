# ECE-2112-PA-1
## Made by: Hera Marishka Aquino | 2-ECE-C
Programming Assignment 1 for Advanced Computer Programming (S.Y. 2026-2027). It includes solutions to three Python problems focusing on Module 1: Base Computing with Python

# 1. Word Problem Rotation
Write a function `rotate_word()` that takes a non-empty string and returns a new string with the first letter moved to the back. Keep all other characters and their original capitalization intact.
```python
def rotate_word(text) :
    return text[1:] + text[0]

print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))
print(rotate_word("Hello"))
```


Write a function `make_username(first_name, last_name)` that takes the first and last name and returns a formatted username. The function should:
1. Conv# 2. User Builder Problemert both names to lowercase.
2. Strip out all spaces from both names.
3. Join the processed first and last name with a single (.).
```python
def make_username(first_name, last_name) :
    clean_first = first_name.replace(" ", " ").lower()
    clean_last = last_name.replace(" ", " ").lower()
    return clean_first + "." + clean_last

print(make_username("Ada","Lovelace"))
print(make_username("Alan","Turing"))
print(make_username("Ana Maria","De Leon"))
print(make_username("Ash","Trevino"))
```

# 3. Bookend Swap Problem
Define a function called `swap_bookends(items)` that receives a list of at least two elements and performs the following:
1. Deconstruct the list into three parts: `first` (the starting item), `middle` (all center items on the list), `last` (the ending item).
2. Construct and return a non-mutating copy of the list where the initial and final elements are swapped while preserving the sub-list `middle`.
3. Use the extended sequence unpacking in the following form: `first, *middle, last = items`
```python
def swap_bookends(items) :
    first, *middle, last = items
    return [last] + middle + [first]

print(swap_bookends([1, 2, 3, 4, 5, 6]))
print(swap_bookends(["red", "green", "blue"]))
print(swap_bookends([8, 3]))
```

Thank you so much for reading!

