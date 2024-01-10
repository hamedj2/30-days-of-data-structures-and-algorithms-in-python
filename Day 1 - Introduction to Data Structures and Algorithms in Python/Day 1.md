<img src='../Files/Images/Header.jpg'>

# Day 1

# Python Overview:
Python, renowned for its readability and efficiency, is a high-level, interpreted language. It's famed for its simplicity, making it an excellent choice for beginners, yet powerful enough for complex applications.

## Installing Python:

<img src='/Files/Images/windows-icon.png' width='30' align='center'> </img> **Windows:** 
Download from [python.org](https://www.python.org/downloads/windows/), choose the installer, and follow the prompts. Ensure you tick 'Add Python to PATH'.

<img src='/Files/Images/mac-icon.png' width='30' align='center'> </img> **MacOS:** 
Use [python.org](https://www.python.org/downloads/macos/) to install on macOS or use [Homebrew](https://docs.brew.sh/Homebrew-and-Python) -> `brew install python`.

<img src='/Files/Images/Linux-icon.png' width='30' align='center'> </img>
**Linux:** Python is usually pre-installed. Verify by typing `python3 --version` in the terminal. If not, use your package manager, like `sudo apt install python3` for Ubuntu.

# Python Basics and Operations

## Arithmetic Operations

- [ ] Addition -> ` + ` <br>
- [ ] Subtraction -> ` - ` <br>
- [ ] Multiplication -> ` * ` <br>
- [ ] Division -> ` / ` Divides one number by another, yielding a _floating-point_ result. <br>
- [ ] Floor Division -> ` // ` Performs division but rounds down to the nearest _integer_. <br>
- [ ] Modulus -> ` % ` Returns the remainder of a division. <br>
- [ ] Exponentiation -> ` ** ` Raises a number to the power of another number. <br>

<details>
<summary>
<strong>Examples for Arithmetic Operations</strong>  
</summary>
   
```python
print(5 + 3)  # 8
print(10 - 2)  # 8
print(4 * 2)  # 8
print(16 / 2)  # 8.0
print(17 // 2)  # 8
print(18 % 10)  # 8
print(2 ** 3)  # 8
```

</details>


## Comparison Operations

- [ ] Equal -> ` == ` Checks if two values are equal. <br>
- [ ] Not Equal -> ` != ` Checks if two values are not equal. <br>
- [ ] Greater Than -> ` > ` Checks if the first value is greater than the second. <br>
- [ ] Less Than -> ` < ` Checks if the first value is less than the second. <br>
- [ ] Greater Than or Equal To -> ` >= ` Checks if the first value is greater than or equal to the second. <br>
- [ ] Less Than or Equal To -> ` <= ` Checks if the first value is less than or equal to the second. <br>

<details>
<summary>
<strong>Examples for Comparison Operations</strong>  
</summary>
  
```python
print(8 == 8)  # True
print(7 != 8)  # True
print(9 > 8)  # True
print(7 < 8)  # True
print(8 >= 8)  # True
print(8 <= 8)  # True
```
</details>

## Logical Operations

- [ ] And -> ` and ` Returns True if both operands are true. <br>
- [ ] Or -> ` or ` Returns True if at least one operand is true. <br>
- [ ] Not -> ` not ` Negates the boolean value. <br>

<details>
<summary>
<strong>Examples for Logical Operations</strong>  
</summary>
  
```python
print(True and False)  # False
print(True or False)  # True
print(not True)  # False
```
</details>

## Bitwise Operations



- [ ] AND -> ` & ` Performs a bitwise AND. <br>
- [ ] OR -> ` | ` Performs a bitwise OR. <br>
- [ ] XOR -> ` ^ ` Performs a bitwise XOR. <br>
- [ ] NOT -> ` ~ ` Performs a bitwise NOT. <br>
- [ ] Left Shift -> ` << ` Shifts bits to the left. <br>
- [ ] Right Shift -> ` >> ` Shifts bits to the right. <br>

<details>
<summary>
<strong>What Are Bitwise Operations?</strong>  
</summary>

- `AND (&):` Compares two numbers bit by bit. The result is 1 for each bit where both numbers have a 1. Otherwise, it's 0.  
Example: For 5 (101 in binary) & 3 (011 in binary), only the last bit matches (1 & 1 = 1), so the result is 001 or 1 in decimal.

- `OR (|):`Compares bit by bit. If at least one of the two numbers has a 1 in a particular position, the result gets a 1 in that position.  
Example: For 5 (101 in binary) | 3 (011 in binary), the result is 111 or 7 in decimal, since in each position at least one of the numbers has a 1.

- `XOR (^):` This is a bit like OR, but if both numbers have a 1 in the same position, the result gets a 0 in that position.  
Example: For 5 (101 in binary) ^ 3 (011 in binary), the result is 110 or 6 in decimal. This is because the first and last bits are different in the two numbers.

- `NOT (~):`This flips all the bits of a number. If a bit is 1, it becomes 0, and vice versa.
Example: For ~5, every bit in 5 (101 in binary) is flipped, resulting in 010 in binary (or 2 in decimal, but note that Python handles this operation a bit differently due to how it represents negative numbers).

- `Left Shift (<<):` Moves all the bits in a number to the left by a certain number of places (specified by you). This is like multiplying the number by 2 for each shift.  
Example: 5 (101 in binary) shifted left by 1 place (1010 in binary) is 10 in decimal.

- `Right Shift (>>):` Moves all the bits in a number to the right by a certain number of places. This is like dividing the number by 2 for each shift.  
Example: 5 (101 in binary) shifted right by 1 place (010 in binary) is 2 in decimal.
```python
print(5 & 3)  # 1
print(5 | 3)  # 7
print(5 ^ 3)  # 6
print(~5)  # -6
print(5 << 1)  # 10
print(5 >> 1)  # 2
```
</details>

