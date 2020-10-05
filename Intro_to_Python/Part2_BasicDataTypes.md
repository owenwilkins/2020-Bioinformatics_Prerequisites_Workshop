# Part 2: Basics of Python and Basic Data Types

## Outline 
- [Basic data types](#datatypes)
- [Basic arithmetic](#arithmetic)
- [Comparisons](#comparisons)
- [Basic data structures](#datastructures)
- [Boolean Operations](#operations)
- [Range](#range)
- [String Formatting](#stringformat)
- [Group Exercise](#exercise)


---

# <a name="datatypes"></a> Basic Data Types: Integers, Floating-point numbers, booleans, strings.

## Integers

```
a = 1
type(a)
a
```
<div class="output">>>> a = 1
>>> type(a)
<class 'int'>
>>> a
1

</div>


## Floats

```
b = 1.2
type(b)
b
```

<div class="output">>>> b = 1.2
>>> type(b)
<class 'float'>
>>> b
1.2
</div>


## Booleans

"In computer science, the Boolean data type is a data type that has one of two possible values (usually denoted true 
and false) which is intended to represent the two truth values of logic and Boolean algebra. It is named after George 
Boole, who first defined an algebraic system of logic in the mid 19th century." [-wikipedia](https://en.wikipedia.org/wiki/Boolean_data_type)

```
c = True
d = False
type(c)
c
int(d)
# TODO float(d), long(d),
```

<div class="output">>>> c = True
>>> d = False
>>> type(c)
<class 'bool'>
>>> c
True
>>> int(d)
0
</div>

## Strings
```
my_string = "Hello world!"
type(my_string)
my_string
print(my_string)
my_string[1] # this will make more sense when we learn lists later
```



# <a name="arithmetic"></a> Arithmetic: Adding, subtracting, multiplication, etc.

```
# This is a comment
type(a)
type(b)

# Addition
a + b
type(a+b)

# Subtraction
b - a
type(b-a)

# Division
a/b
type(a/b)

# Exponents
4**b
type(a**b)

# TODO (//, abs, pow(x,y))

```

<div class="output">>>> # This is a comment
>>> type(a)
<class 'int'>
>>> type(b)
<class 'float'>
>>> 
>>> # Addition
>>> a + b
2.2
>>> type(a+b)
<class 'float'>
>>> 
>>> # Subtraction
>>> b - a
0.19999999999999996
>>> type(b-a)
<class 'float'>
>>> 
>>> # Division
>>> a/b
0.8333333333333334
>>> type(a/b)
<class 'float'>
>>> 
>>> # Exponents
>>> 4**b
5.278031643091577
>>> type(a**b)
<class 'float'>
</div>


## A few other things

```
a += 1
a

a -= 1
a
```

<div class="output">
>>> a += 1
>>> a
2
>>> 
>>> a -= 1
>>> a
1
</div>

# <a name="comparisons"></a> Comparisons: <, >, <= , >= , ==,

```
1<1
1<2
2>1
1<=1
2>=1
1==1
0==1
```

<div class="output">
>>> 1<1
False
>>> 1<2
True
>>> 2>1
True
>>> 1<=1
True
>>> 2>=1
True
>>> 1==1
True
>>> 0==1
False

</div>

# <a name="datastructures"></a> Basic Data Structures: Lists, Sets, Tuples, Dictionaries.

## Lists
```
my_list = [1,2,3,4,5,6]
type(my_list)

# getting the first element in a list (0 index)
my_list[0]

# getting the last element in a list
my_list[-1]
# OR
my_list[5]

# getting a range of the list
my_list[-3:]
my_list[1:3]
my_list[:3]

# some other features of integer lists
sum(my_list)
len(my_list)

my_list2 = [7,8,9]

# adding and subtracting lists
my_list+my_list2
my_list-my_list2


# string lists, double indexing
my_string_list = ['the', 'dog', 'says', 'woof']
my_string_list[0][1:]

# join, splits, replace, 
" ".join(my_string_list)
list(my_string_list[0])
" ".join(my_string_list).split()

```

<div class="output">
>>> my_list = [1,2,3,4,5,6]
>>> type(my_list)
<class 'list'>
>>> 
>>> # getting the first element in a list (0 index)
>>> my_list[0]
1
>>> 
>>> # getting the last element in a list
>>> my_list[-1]
6
>>> # OR
>>> my_list[5]
6
>>> 
>>> # getting a range of the list
>>> my_list[-3:]
[4, 5, 6]
>>> my_list[1:3]
[2, 3]
>>> my_list[:3]
[1, 2, 3]
>>> 
>>> # some other features of integer lists
>>> sum(my_list)
21
>>> len(my_list)
6
>>> 
>>> my_list2 = [7,8,9]
>>> 
>>> # adding and subtracting lists
>>> my_list+my_list2
[1, 2, 3, 4, 5, 6, 7, 8, 9]
>>> my_list-my_list2
Traceback (most recent call last):
  File 
TypeError: unsupported operand type(s) for -: 'list' and 'list'
>>> 
>>> 
>>> # string lists, double indexing
>>> my_string_list = ['the', 'dog', 'says', 'woof']
>>> my_string_list[0][1:]
'he'
>>> 
>>> # join, splits, replace, 
>>> " ".join(my_string_list)
'the dog says woof'
>>> list(my_string_list[0])
['t', 'h', 'e']
>>> " ".join(my_string_list).split()
['the', 'dog', 'says', 'woof']

</div>


## Tuples


```
my_tuple = (1,2,3,4,5,6)
type(my_tuple)

# getting the first element in a tuple (0 index)
my_tuple[0]

# getting the last element in a tuple
my_tuple[-1]
# OR
my_tuple[5]

# getting a range of the tuple
my_tuple[-3:]
my_tuple[1:3]
my_tuple[:3]

my_tuple2 = (7,8,9)

# adding and subtracting tuples
my_tuple+my_tuple2
my_tuple-my_tuple2
```

<div class="output">
>>> my_tuple = (1,2,3,4,5,6)
>>> type(my_tuple)
<class 'tuple'>
>>> 
>>> # getting the first element in a tuple (0 index)
>>> my_tuple[0]
1
>>> 
>>> # getting the last element in a tuple
>>> my_tuple[-1]
6
>>> # OR
>>> my_tuple[5]
6
>>> 
>>> # getting a range of the tuple
>>> my_tuple[-3:]
(4, 5, 6)
>>> my_tuple[1:3]
(2, 3)
>>> my_tuple[:3]
(1, 2, 3)
>>> 
>>> my_tuple2 = (7,8,9)
>>> 
>>> # adding and subtracting tuples
>>> my_tuple+my_tuple2
(1, 2, 3, 4, 5, 6, 7, 8, 9)
>>> my_tuple-my_tuple2
Traceback (most recent call last):
  File 
TypeError: unsupported operand type(s) for -: 'tuple' and 'tuple'
</div>

## Tuples vs Lists

```
my_list[0] = 135
my_list
my_tuple[0] = 135
my_tuple

```
<div class="output">
>>> my_list = [1,2,3,4,5,6]
>>> my_list[0] = 135
>>> my_list
[135, 2, 3, 4, 5, 6]
>>> my_tuple[0] = 135
Traceback (most recent call last):
  File
TypeError: 'tuple' object does not support item assignment
>>> my_tuple
(1, 2, 3, 4, 5, 6)

</div>

## Sets

```
my_set = {1,2,3,4,5,5}
my_set
#OR 
my_set = set([1,2,3,4,5,5]) 
my_set
type(my_set)


# Can we index sets like we do lists? No
my_set[0]


my_set2 = {5,7,8,9}

# intersection and union of sets etc.

# union
my_set|my_set2
# intersection
my_set&my_set2
# subtracting sets
my_set-my_set2
my_set2-my_set

```


<div class="output">

>>> my_set = {1,2,3,4,5,5}
>>> my_set
{1, 2, 3, 4, 5}
>>> #OR 
>>> my_set = set([1,2,3,4,5,5]) 
>>> my_set
{1, 2, 3, 4, 5}
>>> type(my_set)
<class 'set'>
>>> 
>>> 
>>> # Can we index sets like we do lists? No
>>> my_set[0]
Traceback (most recent call last):
  File 
TypeError: 'set' object is not subscriptable
>>> 
>>> 
>>> my_set2 = {5,7,8,9}
>>> 
>>> # intersection and union of sets etc.
>>> 
>>> # union
>>> my_set|my_set2
{1, 2, 3, 4, 5, 7, 8, 9}
>>> # intersection
>>> my_set&my_set2
{5}
>>> # subtracting sets
>>> my_set-my_set2
{1, 2, 3, 4}
>>> my_set2-my_set
{8, 9, 7}
</div>

## Dictionaries
```
my_dict = {'a':1, 'b':2, 'c':3}
type(my_dict)

my_dict.keys()
my_dict.values()
my_dict['a']
```

<div class="output">
>>> my_dict = {'a':1, 'b':2, 'c':3}
>>> type(my_dict)
<class 'dict'>
>>> 
>>> my_dict.keys()
dict_keys(['a', 'b', 'c'])
>>> my_dict.values()
dict_values([1, 2, 3])
>>> my_dict['a']
1
</div>


# <a name="operations"></a> Boolean Operations: and, or, not 

```
1 and 1
0 and 1
0 or 1 
not 1
not 0
not True
not False
True and False
True or False
```

<div class="output">
>>> 1 and 1
1
>>> 0 and 1
0
>>> 0 or 1 
1
>>> not 1
False
>>> not 0
True
>>> not True
False
>>> not False
True
>>> True and False
False
>>> True or False
True

</div>

# <a name="range"></a> Range

# <a name="exercise"></a> Group Exercises (~30 mins)
1. Create a list of all even values from 0 to 100.
- What is the length of the list?
- What is the average of the list?  
- What is the sum of the 13 to the 17th elements in the list?
- What is the 16th element from the end?
- Replace the 23rd element with the value 200. Now what is the average?


2. Learning to use python it is good to have an experimental mentality to learn more about edge cases
- What is the empty list in terms of a boolean value?
- What is an empty dictionary in terms of a boolean value?
- What about a float value of 0?


3. Create a string in python with some information about yourself (Name, background, etc.) 
- Take the string you created and make a list out of it where each word is an element.
- Now recreate the string with two spaces where there was originally one space. There are two ways, one using the list 
and one using the original string. Can you think of both?


4. 




<div class="output">
 
</div>

<div class="output">
 
</div>

<div class="output">
 
</div>
- reverse lists etc., step size in lists [::2], any, all
-  pop and append lists etc....
-  rounding
-  Single and double quotes, escape characters, etc TODO
-  inserting variables TODO
-  Zero-based index, variables vs objects
-  Maybe Counter() and OrderedDict() from collections (https://docs.python.org/2/library/collections.html)


*  Part 2: Hands on exercises (1:30 - 2pm)
    -  TODO

