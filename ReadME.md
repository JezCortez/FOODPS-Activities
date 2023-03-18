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

### Integer
Integer or `int` is a data type used for any whole numbers like 5, 400 or 1000, basically any number that isn't derived from a fraction is a whole number, this also includes negative numbers.

### Floating Point
Floating point or `float` is a data type used for fractions or fraction of a number that comprises of a decimal point, numbers like 3.14, 5.977 or 300.0.

### String
String or `str` is a data type used for ordered sequence of characters. It is commonly used with words and phrases and is the default data type in a `print` function. Example of a string would be: "hello", "goodbye" and "blah blah blah". Spaces, numbers and symbols and any combination of these can be used in a string.

### List
List or `list` is a data type used to make an ordered sequence of objects, objects can be of other data types such as the Integer, Floating Point or String. The order is numbered from the first object starting from 0 then 1, 2, 3 and so on. The syntax of the list data type is `[]` Brackets.

### Dictionary
Dictionary or `dict` is a date type used to make an unordered pairs of keys with their respective values. Keys of a dictionary is always a string but the values can be of any data type. The syntax of a dictionary are `{}` Curly Brackets with `:` a Colon indicating the value of the key.

### Tuple
Tuple or `tup` is a data type much like the list in where it is an ordered sequence of objects, but a Tuple is different in the sense that it is immutable or unchangeable. A Tuple can be other data types like Integer, Floating point or String.

### Set
Set or `set` is a data type used to make unordered set of unique objects, it is unchangeable and does not allow duplicates, however, you can add or remove items of a set. The syntax of a set is the same with the dictionary, `{}` Curly Brackets.

### Boolean
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

## Activity #3: Slice your name
A value of a String can be manipulated and this activity is a good example of the many things you can do with String.

```python
name="Random Name"

print(name[1:5])
print(name[8:10])
```
In this code, the goal is to slice your name in a way where it removes the first and last letter of you first, middle and last name, for this, we will be using String Indexing.
 
String indexing is sort of a way to "slice" a string. Indexing uses `[]` brackets for the notation after the String or a variable assigned to the string.

`[Start:Stop:Step]` is the syntax of String indexing. The "Start" is the numerical index to indicate the start of the slice, the "Stop" is where it ends (the value in this index won't be added) and "Step" is the amount of units it "jumps" at.

The output of this would be:
```python
ando
am
```

## Tuple as key in dictionary
Tuple can be used as a key in a Dictionary, since it is an ordered sequence while being immutable, it is perfect in a use case where you want the "keys" to not alter or fail.

```python
mytups=("1","2","3")

keys={mytups[0]:"Hello", mytups[1]:"Hi", mytups[2]:"Good Morning"}

print(keys["1"])

```
This program is able to print a value of a key by just calling the key in the `print()` function, which can make it really organized and easily expandable.

This part is where the tuples are defined. Here, each tuple is a key to a value and is named "1", "2" and "3".
```python
mytups=("1","2","3")
```

This is where the values of the keys are stored, as a dictionary, following a index method of calling a tuple key, in this case, "1" would be numerical index 0, then "2" is 1 and so on.
```python
keys={mytups[0]:"Hello", mytups[1]:"Hi", mytups[2]:"Good Morning"}
```



```python
print(keys["1"])

```
In the `print()` function, we can set what value to output by putting the key of that value, in the example of `keys["1"]`, the output would be 
```python
Hello
```

## If Problems

If statements are conditional operations where it does something in some condition.
`if`, `elif` and `else` is part of the If statements.

It follows a control flow syntax and here is how it is used:
```python
if some_condition:
    execute_this
elif other_condition:
    execute_other_things
else:
    do_something_else
```
### Comparison Operators
Comparison operators are used for comparing two different values with each other.

#### [ == ]
`==` or "Equal To" makes a condition true if both of the values compared are equal to each other.
#### [ != ]
`!=` or "Not Equal To" makes a condtion true if both of the values compared are not equal to each other. 
#### [ > ]
`>` or "Greater Than" makes a condtiion true if the left operand is greater than the right operand.
#### [ < ]
`<` or "Less Than" makes a conditions true if the left operand is less than the right operand.
#### [ >= ]
`>=` or "Greater Than or Equal To" makes a condition true if the left operand is greater than or equal to the right operand.
#### [ <= ]
`<=` or "Less Than or Equal To" makes a condition true if the left operand is less then or equal to the right operand.


### 1. Positive and Negative Numbers
The assignment is to write a program that asks a user to input a number and checks if the number is positive or negative.

The program below does exactly as what is asked for:
```python
num = int(input("enter a number: "))

if num % 2==0:
    print("The Number is Even")

else:
    print("The Number is Odd")
```
This part prompts a user to input a number, we set it to only accept integers.
```python
num = int(input("enter a number: "))
```
After we get an input, this part is where we have our if-else statement.
```python
if num % 2==0:
    print("The Number is Even")
    
else:
    print("The Number is Odd")
```
The `%` percent symbol is a Modulo Operator, it divides the left hand operand to the right hand operand and returns the remainder. If the left hand operator can be evenly divided, the returned value is 0 and if there is a remainder, the value will be 1.

Since an evenly divided left hand operand nets 0 value, we can use it to check if a number is even or odd. A definition of an even number is a number that can be evenly divided by 2 so in our if statement:

```python
if num % 2==0:
    print("The Number is Even")
```
We use the `%` percent symbol to know if the number inputted divided by 2 is evenly divided which has the value of 0, in that case, it prints "The number is Even", if it isn't equal to 0, it goes to the else function:

```python
else:
    print("The Number is Odd")
```
If the outcome of the previous operation didn't fulfill the conditions set, it goes to the else function, in this case, it prints "The number is odd"


### 2. Age
The assignment is to write a program that asks a user to input their age and checks whether they are of legal age (18 years old)
```python
age = int(input("How old are you?: "))

if age >= 18:
    print("Old Enough")

else:
    print("Not Old Enough")
```
Same format as no. 1, we will use a comparison operator, in this case, we will use the greater than/equal to comparison operator.
```python
if age >= 18:
    print("Old Enough")
```
It will compare if the input of the user is greater than or equal to 18 and print "Old Enough", if the condition isn't met, it will go to the else function and print "Not Old Enough".
```python
else:
    print("Not Old Enough")
```

### 3. Two Equal numbers
The assignment is to write a program where the user inputs two numbers and checks if the two numbers are equal.
Same with no.1, we will use the equal to comparison operator.
```python
num1 = int(input("Input the First Number: "))
num2 = int(input("Input the Second Number: "))

if num1 == num2:
    print("Both numbers are equal")

else:
    print("The numbers are not equal")
```
We assign a variable to each number for each input and we compare them together to check if both of them are equal to each other.

### 4. Name Length
We can use the `len()` function to count how many characters are there in a String.
```python
name = input("What is your name?: ")

if len(name) > 10:
    print("Name is longer than 10 Characters. The length is:", len(name))    
else:
    print("Name is not longer than 10 Characters. The length is:", len(name))
```
We can put the `len()` function in an if statement, in this case, we need to use a comparison operator to compare if the name inputted is longer than 10 characters.
```python
if len(name) > 10:
```
Depending on the outcome, it will print the appropriate output. In both the if and else statements, we can add the `len()` function to the print so that it indicates how many characters are there.
```python
print("Name is longer than 10 Characters. The length is:", len(name))    
else:
    print("Name is not longer than 10 Characters. The length is:", len(name))
```

### 5. Gender
We can also use comparison operators to check if a String is equal to another String. `.lower()` is a python method wherein we can change the whole String to be lowercase letters, which will make the comparison between Strings easier.
```python
gender = input("What is your gender?: ").lower()

if gender == 'male':
    print("Your gender is: Male")

elif gender == 'female':
    print("Your gender is: Female")

else:
    print("Error")
```

To compare Strings, the expected value should be enclosed in `''` apostrophe.
```python
if gender == 'male':
```
We do the same thing with 'female', but this time, we use elif as it is another condition that we are considering.
```python
elif gender == 'female':
```
And of course else will print error.






## Topic 3.1: Tatsulok!
`for` is a type of loop in python where it is used to iterate over a sequence, while `range()` is a function that returns a sequence of numbers, starting from 0, and increments by 1, and stops at a specified number.
```python
n = int(input("Please input the highest point of the triangle: "))
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


## Palindrome
The objective is to write a program that checks if the user inputted word is a palindrome or not.
Since a palindrome is a word that is the same reversed, flipping the word and comparing it to the original word is a good way to do it.

```python
x = input("Input a word: ").lower()

if x == x[::-1]:
    print("The word is a palindrome")
else:
    print("The word is not a palindrome")
```
Same as the others, the first part asks for a user input, with `lower()` method where each character of the world is going to be changed to lowercase letters.
```python
x = input("Input a word: ").lower()
```
The line wwhere it checks the palindrome does two things, first, it uses a comparison operator for confirmation and second, it also uses String formatting. `[::-1]` flips the string backwards just as highlighted in [activity #3](https://github.com/JezCortez/FOODPS-Activities/blob/main/ReadME.md#activity-3-slice-your-name) where the "step" part goes backward with no start or end in the "slice". It prints "The word is a palindrome" if the conditions are true and "The word is not a palindrome" if its false.





