# Python-Cheatsheet

# Contents
--------
1. **Data Types:** 
  * __[`Numeric Data Type`](#numeric-data-type)__
  * Sequence Data Type:**__[`Strings`](#strings)__,__[`Lists`](#lists)__,__[`Tuples`](#tuples)__**
  * __[`Boolean Data Type`](#boolean-data-type)__
  * __[`Sets`](#sets)__
  * __[`Dictionaries`](#dictionaries)__
  * __[`None`](#none)__
2. **Opeartors**
  * __[`Basic Operators`](#basic-operators)__
4. **Loops**
5. **Functions**
6. **Advanced Python**

## Data Types
----
Numeric Data Type
----
* **It consists of int (integers), float (floating point numbers) and complex numbers**
* **type() is used to determine the data type**
```python
type(10)   # int 
type(-10)  # int
type(10.0) # float
type(27.5) # float
type(2+3J) # complex
```

### Sequence Data Type
* **It is a ordered collection of similar or different data types**
----
Strings
----
* **It is a collection of one or sequence of characters in memory**
* **There is no character data type in python, a string of length one can be considered as a character** 
```python
type('Hello World') # str

#To print single quote(') use \' or write it within double quotes
'I\'m Subathra'
"I'm Subathra"
# Use triplr quotes to write multiple lines
'''Subathra
   Chinu'''
```
* Characters in the string are accesed by indexing[]
```python
name='subathra'
name[4]  # t
name[0]  # s
name[-1] # a
```
![alt text](https://github.com/Subathra19/Python/blob/main/images/string.PNG)
----
Lists
----
* **An ordered collection of different items.**
* **Lists are mutable (i.e.) values can be changed during the course of program**
```python
a = []                           # Empty list
a = [10, 20.1, "Hello"]
a = [10, 20.1, "Hello", [1,5.2]] # Nested list
```
* Lists can also be created using range(start,stop,step)
```python
a = list(range(1,5)) # [1, 2, 3, 4]
a = list(range(1,5,2)) # [1, 3]

```
* Elements of list can be accessed using indexing[] (similar to string) 
```python
a = [10, 20.1, "Hello", [1,5.2]]
a[0] # 10
# To access from nested list
a[-1][0] # 1
```
----
Tuples
----
* **It ia also an ordered collection of different items.**
* **But Tuples are immutable (i.e.) values can't be changed during the course of program**
```python
a = ()   # Empty Tuple
a = (1)  # Not a Tuple
a = (1,) # It is a tuple
a = (10, 20.1, "Hello", (1, 5.2)) # Nested tuple
```

* Elements of tiple can be accessed using indexing[] 
```python
a = (10, 20.1, "Hello", (1,5.2))
a[1] # 20.1
# To access from nested list
a[-1][-1] # 5.2
```

Boolean Data Type
----
* **It has two built-in values: True or False**
* **It is used in comparison and logical operations in Python**
```python
type(True)  # bool
type(False) # bool
type(true)  # It is not a boolean data type. We get error
```

Sets
---
* **It is an unorderd collection of unique elements (i.e) no duplicate elements.**
* **It is mutable**
```python
a = set()               # Empty set
set(1,2,3)              # {1,2,3}
set("subathra")         # {'b', 't', 's', 'h', 'r', 'a', 'u'}
set([1,2,"subathra",0]) # {0, 1, 2, 'subathra'} --> Integer followed by string
```

Dictionaries
----------
* **It is an ordered collection of data values. Stores the data values like a map.**
* It holds key value pairs for optimization**
```python
a = {}     #Empty dictionary
a = {'Name':'Subathra','Id':32}
a.values() # ['Subathra',32]
a.keys()   # ['Name','Id']
```

None
----
**None is used to define a null value (i.e.) absence of a value**
```python
a = None   # nothing has been assigned
type(None) # NoneType
```
----
## Operators
----
Basic Operators
----
**Arithmetic Operators**
```python
+  # Adds two operands
-  # Subtracts right operand from left operand
*  # Multuplies two operands
/  # Divides left operand by hand operand and returns quotient
%  # Divides left operand by hand operand and returns remainder
** # Exponrntial operation (i.e.) returns first raised to power second
// # Floor division (i.e.) divides left operand by hand operand and returns floor of quotient
```
**Comparison Operators**
```python
== # Both operands are equal
!= # Both operands are not equal
>  # Left operand is greater than right operand
<  # Left operand is less than right operand
>= # Left operand is greater than or equal to right operand
<= # Left operand is less than or equal to right operand
```

**Assignment Operators**
```python
=   # Assigns values of right operand to left operand 
+=  # Adds both operand and assign the result to left operand
-=  # Subtracts right operand from left operand and assign the result to left operand
*=  # Multuplies two operands and assign the result to left operand
/=  # Divides left operand by hand operand and assign the quotient to left operand
%=  # Divides left operand by hand operand and assign the remainder to left operand
**= # Performs exponential operation and assign the result to left operand
//= # Performs floor division and assign the result to left operand
```
**Logical Operators**
```python
and # Returns true if both operands are true
or  # Returns true if either of the operands is true
not # Returns the reverse of the logical state of the operand
```
**Bitwise Operators**
```python
&  # Bitwise AND
|  # Bitwise OR
~  # Bitwise NOT
^  # Bitwise XOR
>> # Bitwise right shift
<< # Bitwise left shift
```
**Identity Operators**
```python
<element> is <element>     # Returns true if both operands refer to same object in memory
<element> is not <element> # Returns true if both operands does not refer to same object in memory
```
**Membership Operators**
```python
<element> in <element>     # Returns true if value is found in the sequence
<element> not in <element> # Returns true if value is not found in the sequence
```
Credits
------
Inspired by: https://github.com/gto76/python-cheatsheet

