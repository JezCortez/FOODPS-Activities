# FOODPS-Activities
Fundamentals of Object-oriented Programming and Discrete Structures (FOODPS) Activity Programs

This is a collection for all the programming activities of the AdDU-SHS FOODPS subject. With this, it will guide and explain the code presented as well as show how it works. This can be used to know the codes ahead of time, even also to practice said activities. 


FOODPS uses python3 and when trying any of the codes, copy it and paste it to any python3 IDE like:
- [Visual Studio](https://visualstudio.microsoft.com)
- [Visual Code](https://code.visualstudio.com/download)
- [PyCharm](https://www.jetbrains.com/pycharm/)

or use an [online python compiler](https://www.onlinegdb.com/online_python_compiler)


Since this is part of the assignments in this subject, it is highly recommended to change the variable names of the code so as to not promote plagiarism, although I don't particularly mind about it, it is still good practice to change it in a way that its different from source code.


Sharing of the codes and programs is widely accepted and linking this repository is much appreciated!

## Python Data Types
Here are some Data types that are going to be discussed in the FOODPS subject:
- **Integer**
- **Floating Point**
- **String**
- **List**
- **Dictionary**
- **Tuple**
- **Set**
- **Boolean**

#### Integer
Integer or `int` is a data type used for any whole numbers like 5, 400 or 1000, basically any number that isn't derived from a fraction is a whole number, this also includes negative numbers.

#### Floating Point
Floating point or `float` is a data type used for fractions or fraction of a number that comprises of a decimal point, numbers like 3.14, 5.977 or 300.0.

#### String
String or `str` is a data type used for ordered sequence of characters. It is commonly used with words and phrases and is the default data type in a `print` function. Example of a string would be: "hello", "goodbye" and "blah blah blah". Spaces, numbers and symbols and any combination of these can be used in a string.

#### List
List or `list` is a data type used to make an ordered sequence of objects, objects can be of other data types such as the Integer, Floating Point or String. The order is numbered from the first object starting from 0 then 1, 2, 3 and so on. The syntax of the list data type is `[]` Brackets.

#### Dictionary
Dictionary or `dict` is a date type used to make an unordered pairs of keys with their respective values. Keys of a dictionary is always a string but the values can be of any data type. The syntax of a dictionary are `{}` Curly Brackets with `:` a Colon indicating the value of the key.

#### Tuple
Tuple or `tup` is a data type much like the list in where it is an ordered sequence of objects, but a Tuple is different in the sense that it is immutable or unchangeable. A Tuple can be other data types like Integer, Floating point or String.\

#### Set
Set or `set` is a data type used to make unordered set of unique objects, it is unchangeable and does not allow duplicates, however, you can add or remove items of a set. The syntax of a set is the same with the dictionary, `{}` Curly Brackets.

#### Boolean
Boolean or `bool` is a data type used to indicate if a value is true or false.


 
## Activity #1: Hello world

`print` is one of the simplest and most used function in all of python programming, it allows the program to output anything like a message or an answer.

```python
print("Hello World")
```
In this case, the program will output `Hello World` when executed.

The `print` function has two parts:
The function itself
```python
print()
```
and the parameters
```python
("Hello World")
```
The function is straightforward, it calls for a function, in this case the `print` function to indicate that the program needs to output whatever is inside the parameters section

The parameters are what is to be outputted by the program, which is `"Hello World"`

## Activity #2: Check your Temperature
Assigning a variable is important in this case as it can be used in mathematical operations.
```python
f=float(input())
c=(5/9)*(f-32)

print(c)
```
In the code above, we are using two variables, `f` and `c` to solve for what is asked.
The `f` variable is for the input of the user, which also indicates that it accepts `float` input. 
```python
f=float(input())
```

Meanwhile the `c` variable is for the equation. Notice that the `f` variable is being used in the equation in order to get an answer.
```python
c=(5/9)*(f-32)
```

And of course, it prints the outcome.
```python
print(c)
```

## Topic 3.1: Tatsulok!
`for` is a type of loop in python where it is used to iterate over a sequence, while `range()` is a function that returns a sequence of numbers, starting from 0, and increments by 1, and stops at a specified number.
```python
n = int(input("Please input the highest point of the triangle "))
for r in range(n):
    for c in range(r + 1):
        print('*', end="")
    print()

for r in range(n):
    for c in range(n - r - 1):
        print('*', end="")
    print()
```
In this instance, this makes a triangle out of asterisks with the number that we indicate to be the number of asterisks at the highest point of the triangle.
The first part is to get the user input for the highest point of the triangle.
```python
n = int(input("Please input the highest point of the triangle "))
```
Next is where the `for` loop and `range()` function is used.
```python
for r in range(n):
```
Basically, the program will loop until the `range()` of variable `n`, or in this case, the user input.
```python
   for c in range(r + 1):
       print('*', end="")
   print()
```
The inner loop or the loop inside the other loop where it adds +1 to variable `r` is there to add an aditional asterisk every time the first loop loops, it also prints the asterisk and ends with no space. The last print is for the program to move on to the next line after the previous.

The second part is the inverse of the first part, instead of adding asterisks, it subtracts 1.
```python
for r in range(n):
    for c in range(n - r - 1):
        print('*', end="")
    print()
```
Same function as before, but now, every loop subtracts 1 asterisk until the variable `n` reaches 0.
