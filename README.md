# Python-Cheatsheet

# Contents

1. **Data Types:** 
  * __[`Numeric Data Type`](#numeric-data-type)__
  * Sequence Data Type:**__[`Strings`](#strings)__,__[`Lists`](#lists)__,__[`Tuples`](#tuples)__**
  * __[`Boolean Data Type`](#boolean-data-type)__
  * __[`Sets`](#sets)__
  * __[`Dictionaries`](#dictionaries)__
  * __[`None`](#none)__
2. **Opeartors**
  * __[`Basic Operators`](#basic-operators)__
  * __[`Basic Operations`](#basic-operations)__
4. **Conditionals and Loops**
  * __[`Conditionals`](#conditionals)__
  * __[`Loops`](#loops)__   
6. **Functions**
7. **Advanced Python**
----
## Data Types

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

Strings
----
* **It is a collection of one or sequence of characters in memory**
* **There is no character data type in python, a string of length one can be considered as a character** 
```python
type('Hello World') # str

#To print single quote(') use \' or write it within double quotes
'I\'m Subathra'
"I'm Subathra"
# Use triple quotes to write multiple lines
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
Basic Operations
----
* dir() is a built-in function, used to return the list of the attributes and methods of any object.

**Basic functions of Numeric data type**
```python
pow(a,b)         # a**b
abs(-a)          # a
round(10.58)     # 10
round(10.5935,2) # 10.59 --> round to 2nd digit
bin(10)          # '0b1010' --> Returns the binary equivalent
hex(512)         # '0xa' --> Returns the hexadecimal equivalent
```
**Basic functions of string**
```python
len('subathra') # 8 --> Returns the number of characters in a string
# Basic Methods
'I'm Subathra'.replace('Subathra', 'Chinu') # 'I'm Chinu' --> Replaces first parameter with second parameter
'Hello world'.split()      # ['Hello', 'world']
'hello world'.upper()      # HELLO WORLD --> Converts the string to upper case
'HELLO WORLD'.lower()      # hello world --> Converts the string to lower case
'hello world'.capitalize() # 'Hello world' --> Converts the first character of a string to upper case
'hello world'.title()      # 'Hello World' --> Converts the first character of each word of a string to upper case
'hello world'.index('d')   # 10 --> Returns the index of the given character
'Hello world'.find('o')    # 4 --> Returns the starting index position of the first occurrence
'hello world'.startswith('hello') # True
'hello world'.endswith('world')   # True
''.join(my_list) # Join all the strings specified in the list with the character specified inside ''

# String formatting
'Hi {}, {}'.format('Subathra','Devi') # Hi Subathra devi
```
**Basic functions of Lists**
```python
len(my_list) # Returns the number of elements in the list
min(my_list) # Returns the minimum element of the list
max(my_list) # Returns the maxiimum element of the list
sum(my_list) # Returns the sum of all elements of the list

# Add an element to the list
my_list.append(<element>)          # Adds the element at the end of the list
my_list.insert(position,<element>) # Adds the element at the given position of the list
my_list.extend(list2)              # Extends the list and adds the values of list2

new_list=list.copy # Copies the elements of list to new_list

# Remove elements from the list
my_list.pop()     # 3 --> Removes and return the last item of the list [mutates the original list]
my_list.pop(1)    # 2 --> Removes and return the item of the list at position 1 [mutates the original list]
my_list.remove(<element>) # Removes the specified element from the list
my_list.clear() # Removes all the elements from the list

# Ordering a list
my_list.sort()             # Mutates the list where the elements of list are sorted in ascending order
my_list.sort(reverse=True) # Mutates the list where the elements of list are sorted in descending order
my_list.reverse() # Mutates the list where the position elements are reversed

# Slicing of list
# Acces a specific range of list using [start:end:step]
a=[1, 2, 3, 4, 5]
a[:3]  # [1, 2, 3] --> Access first three items of list
a[-2:] # [4, 5] --> Access last two items of list
a[1:4] # [2, 3, 4]

# List Comprehension
# To create a new list from other iterables like Tuple, strings, lists, etc.
new_list = [ <action> for <item> in my_list if <condition>] 
new_list = [ <action> if <condition> else <else block> for <item> in my_list] # Order should be maintained else wil get error
```
**Basic functions of Tuples**
```python
len(my_tuple) # Returns the number of elements in the tuple
my_tuple.index(<element>) # Returns the index of an element in tuple
my_tuple.count(<element>) # Returns the number of occurrences of an element in tuple

#Tuples are immutable--> we cannot add or remove elements from the tuple
```
**Basic functions of sets**
```python
# Add an element to the set
my_set.add(<element1>, <element2>)  # {<element1>, <element2>} --> Adds elements to tle list
my_set.add(<element1>)# {<element1>, <element2>} --> no duplicates

# Removes the element from the ser
my_set.remove(<element>)  # Removes the specified element from the set and creates an error if element not found
my_set.discard(<element>) # Removes the specified element from the set and no error if element not found
my_set.clear()            # Removes all the elements from the set

set1.union(set2)        # Combines the elements of both sets into a new set and remove duplicates
set1.intersection(set2) # Returns the elements that are common in both sets
set1.difference(set2)   # Returns the elements that are not common in both sets
set1.issubset(set2)     # Returns True if all the elements of set1 is present in set2
set1.issuperset(set2)   # Returns True if all the elements of set2 is present in set1
set1.isdisjoint(set2)   # Returns True if two sets have a null intersection.

# ZIP() & UNZIP()
# This function is used to map the similar index of multiple entities so that they can be used as a single entity.

name = ["Subathra", "Chinu", "Pooja"]
id = [59, 72, 35]
location = ["India", "Japan", "UK"]
 
# using zip() to map values
a = zip(name, id, location) 
# converting values to set
set(a) # {('Chinu', 72, 'Japan'), ('Pooja', 35, 'UK'), ('Subathra', 59, 'India')}

# To convert the zipped values back to the individual self as they were using * operator
zipped=set(a)
name, id, location = zip(*zipped)
```
**Basic functions of Dictionary**
```python
len(my_dict)           # Returns the number of key-pair values
list(my_dict.keys())   # Creates a list with the keys of dictionary
list(my_dict.values()) # Creates a list with the values of dictionary
my_dict.pop(<key>)     # Removes the key and its corresponding value from the dictionary 
```

----
## Conditionals and Loops

Conditionals
----
* These are the decision making statementsused to decides the flow of program execution.
```python
if condition:           
   Statement1 # Executes if condition is True
statement2 # Executes even if condition fails as it is outside if block
```
```python
if condition:
    # This block gets executed if condition is True
else:
    # This block gets executed if condition is False
```
```python
if condition1:
    # This block gets executed if condition1 is True
elif condition2:
    # This block gets executed if condition2 is True
else:
    # This block gets executed if both conditions are False    
```

Loops
----
* **for loop:**
```python
# for loops are used for sequential search
for <item> in sequence:
    statements
    
# Loop over lists
my_list = [10, 20, 30]
for i in my_list:
    print(i) # 10, 20, 30

# Loop over dictionary items
my_dict = {'Subathra': 123, 'Chinu': 456}
for i in my_dict.keys():
    print(i) # Subathra, Chinu 
for i in my_dict.values():
    print(i) # 123, 456
for i in my_dict.items():
    print(i) # ('Subathra', 123), ('Chinu', 456)
```

* **while loop:**
```python
# Exexutes a block of statements repeatedly until the given condition fails 
while condition:
  statements
```
* **Loop control statements:
```python
continue # Returns control to the begining of loop
break    # Returns the control out of the loop
pass     # To write empty loops, functions
```


Credits
------
Inspired by: https://github.com/gto76/python-cheatsheet

