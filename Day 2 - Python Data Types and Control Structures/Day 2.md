<img src='../Files/Images/Header.jpg'>

# Day 2

<br>
<details>
<summary>
<strong>What is in day 1?</strong>  
</summary>

   - [Data Types](#Data-Types)
      - [Strings]
      - [Integers and Floats]
      - [Lists]
      - [Tuples]
      - [Sets]
      - [Dictionaries]
      
    

</details>


<br>

# Data Types

## Strings

**Definition:** Strings in Python are sequences of characters.

**Creation:** You can create strings using single, double, or triple quotes.

**Immutability:** Once a string is created, it cannot be changed.


**Operations:**
- `Concatenation`: Combining strings using `+`
- `Repetition`: Repeating strings using `*`.
- `Indexing`: Accessing characters by their position.
- `Slicing`: Extracting a part of a string.


**Methods:**
- `.upper()`, `.lower()`: For case conversion.
- `.strip()`: Removing whitespace.
- `.split()`: Splitting a string into a list.
- `.join()`: Joining a list into a string.
- `.replace()`: Replacing parts of a string.
- `.find()`, `.index()`: Finding substrings.

<details>
<summary>
<strong>String Examples</strong>  
</summary

```python

Concatenation = "Hello" + " " + "World!"
Repetition  
    

```

</details>

## Integers and Floats

`Integers`: Whole numbers, positive or negative, without a fractional part.

`Floats`: Numbers with a decimal point.

**Arithmetic Operations:** `+`,` -`, `*`,`/`, `//` (floor division), `%` (modulus), `**` (exponentiation).

Type Conversion: Use `int()` and `float()` to convert between types.

3. Lists
Definition: Ordered, mutable collections of items.
Creation: Using square brackets [].
Operations:
Indexing/Slicing: Access and modify elements.
Appending: .append() to add items.
Extending: .extend() to add multiple items.
Insertion: .insert() to add at a specific position.
Removal: .remove(), .pop(), .clear().
Sorting and Reversing: .sort(), .reverse().
List Comprehensions: Concise way to create lists.
Nested Lists: Lists within lists, useful for matrices.
Usage in Interviews: Dynamic arrays, data storage, iteration.
4. Tuples
Definition: Ordered, immutable collections.
Creation: Using parentheses ().
Usage: Similar to lists but cannot be changed. Often used for data that should not be modified.
Unpacking: Assigning values from a tuple to variables.
Usage in Interviews: Fixed data records, returning multiple values from functions.
5. Dictionaries
Definition: Unordered collections of key-value pairs.
Creation: Using curly braces {} with key-value pairs.
Accessing: Using keys dict[key].
Modification: Add or edit elements by key.
Methods: .keys(), .values(), .items(), .get(), .update().
Nested Dictionaries: Dictionaries within dictionaries.
Dictionary Comprehensions: Create dictionaries using expressions.
Usage in Interviews: Lookup tables, counting problems, JSON data representation.
6. Sets
Definition: Unordered collection of unique elements.
Creation: Using curly braces {} or set() function.
Operations:
Adding Elements: .add().
Removing Elements: .remove(), .discard().
Set Operations: Union, intersection, difference.
Usage: When you need to ensure uniqueness, set operations.
Frozensets: Immutable sets.


----

3. Lists
Indexing/Slicing: Same as strings, but with list elements.
Appending (append(item)): Adds an item to the end of the list.
Extending (extend(iterable)): Adds all elements of an iterable to the list.
Inserting (insert(index, item)): Inserts an item at a specified position.
Removing (remove(item)): Removes the first occurrence of an item.
Popping (pop(index)): Removes and returns an item at the given index.
Sorting (sort()): Sorts the list in place.
Reversing (reverse()): Reverses the list in place.
List Comprehensions: A concise way to create lists. E.g., [x**2 for x in range(10)].
4. Tuples
Indexing/Slicing: Same as lists.
Count (count(item)): Counts the number of occurrences of an item.
Index (index(item)): Finds the first occurrence of an item.
5. Dictionaries
Accessing/Setting (dict[key]): Access or set the value for a key.
Getting (get(key, default)): Returns the value for a key, or default if the key doesn't exist.
Updating (update(other_dict)): Adds key-value pairs from another dictionary.
Keys/Values/Items (keys(), values(), items()): Return views of the dictionary's keys, values, and key-value pairs.
Removing (pop(key)): Removes a key-value pair and returns the value.
Dictionary Comprehensions: Similar to list comprehensions but for dictionaries. E.g., {x: x**2 for x in range(10)}.
6. Sets
Adding (add(item)): Adds an element to the set.
Removing (remove(item)): Removes an element from the set. Raises an error if the element is not present.
Discarding (discard(item)): Removes an element if it is a member. If not, does nothing.
Set Operations:
Union (|): Combines elements from both sets.
Intersection (&): Keeps only elements present in both sets.
Difference (-): Removes elements found in another set.
Symmetric Difference (^): Elements in either set, but not in both.


------

```python

1. Strings
# Concatenation
result = "Hello" + " World"  # "Hello World"

# Repetition
result = "Python" * 3  # "PythonPythonPython"

# Indexing
character = "Python"[0]  # 'P'

# Slicing
substring = "Python"[1:4]  # 'yth'

# Upper and Lower
upper_str = "Python".upper()  # 'PYTHON'
lower_str = "PYTHON".lower()  # 'python'

# Strip
stripped_str = "  Python  ".strip()  # 'Python'

# Split
split_str = "Hello World".split(" ")  # ['Hello', 'World']

# Join
joined_str = "-".join(["Hello", "World"])  # 'Hello-World'

# Replace
replaced_str = "Hello World".replace("World", "Python")  # 'Hello Python'

# Find
index_found = "Hello World".find("World")  # 6

2. Numeric Types (Integers and Floats)

# Arithmetic Operations
sum = 5 + 3  # 8
difference = 5 - 3  # 2
product = 5 * 3  # 15
division = 5 / 3  # 1.666...
floor_division = 5 // 3  # 1
modulus = 5 % 3  # 2
exponentiation = 5 ** 3  # 125

3. Lists

# Creating a List
my_list = [1, 2, 3]

# Indexing/Slicing
element = my_list[0]  # 1
sub_list = my_list[1:3]  # [2, 3]

# Appending
my_list.append(4)  # [1, 2, 3, 4]

# Extending
my_list.extend([5, 6])  # [1, 2, 3, 4, 5, 6]

# Inserting
my_list.insert(0, 0)  # [0, 1, 2, 3, 4, 5, 6]

# Removing
my_list.remove(0)  # [1, 2, 3, 4, 5, 6]

# Popping
popped = my_list.pop(0)  # 1, list is now [2, 3, 4, 5, 6]

# Sorting
my_list.sort()  # [2, 3, 4, 5, 6]

# Reversing
my_list.reverse()  # [6, 5, 4, 3, 2]

# List Comprehensions
squares = [x**2 for x in range(5)]  # [0, 1, 4, 9, 16]

4. Tuples

# Creating a Tuple
my_tuple = (1, 2, 3, 4, 4)

# Indexing/Slicing
element = my_tuple[0]  # 1
sub_tuple = my_tuple[1:3]  # (2, 3)

# Count
count = my_tuple.count(4)  # 2

# Index
index = my_tuple.index(4)  # 3

5. Dictionaries

# Creating a Dictionary
my_dict = {'a': 1, 'b': 2, 'c': 3}

# Accessing/Setting
value = my_dict['a']  # 1
my_dict['d'] = 4  # {'a': 1, 'b': 2, 'c': 3, 'd': 4}

# Getting
value = my_dict.get('e', 5)  # 5

# Updating
my_dict.update({'e': 5})  # {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}

# Keys/Values/Items
keys = list(my_dict.keys())  # ['a', 'b', 'c', 'd', 'e']
values = list(my_dict.values())  # [1, 2, 3, 4, 5]
items = list(my_dict.items())  # [('a', 1), ('b', 2), ('c', 3), ('d', 4), ('e', 5)]

# Removing Elements (pop):
removed_value = my_dict.pop('f')  # 6, and the dictionary is now {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}

# Checking for Key Existence:
has_key_b = 'b' in my_dict  # True

#Dictionary Comprehensions:
squared_dict = {x: x**2 for x in range(4)}  # {0: 0, 1: 1, 2: 4, 3: 9}

#Iterating Over a Dictionary:
for key, value in my_dict.items():
    print(f"Key: {key}, Value: {value}")


6. Sets

Creating a Set:
my_set = {1, 2, 3}
Adding Elements (add):
my_set.add(4)  # {1, 2, 3, 4}
Removing Elements (remove and discard):
my_set.remove(4)  # Removes 4, raises KeyError if not found
my_set.discard(3)  # Removes 3, does nothing if not found
Union (|):
other_set = {3, 4, 5}
union_set = my_set | other_set  # {1, 2, 3, 4, 5}
Intersection (&):
intersection_set = my_set & other_set  # {3}
Difference (-):
difference_set = my_set - other_set  # {1, 2}
Symmetric Difference (^):
symmetric_difference_set = my_set ^ other_set  # {1, 2, 4, 5}
Checking Membership:
is_member = 2 in my_set  # True
Set Comprehensions:
squared_set = {x**2 for x in range(4)}  # {0, 1, 4, 9}
Frozensets: Immutable version of a set.
frozen = frozenset([1, 2, 3])

