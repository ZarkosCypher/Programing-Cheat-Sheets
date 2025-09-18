### Comments: ###
<p>Human readable comments that will not be ran by the machine 
```python
#This is a single line comment
"""
This
Is
A
Multi
Line
Comment
"""
```

```python
print("Hello, World!")
```
```python
print("-" * 50)
#Will print - 50 times one after the other exactly as within the "quotes"
```
```python
#This program will print out "this will print Hello, World!" without the quotes. 
h = "Hello"
w = "World"
print(f"this will print {h}, {w}!")
#The f-string eg f"..." tells Python to interpret {} placeholders as expressions to be evaluated.
a = 2.01
b = 5
print(f"this will print a float 2.0 {a:.1f} and this can also print regular integers {b}.")
#The colon -> : is a format specifier for how a value should be displayed 
#The .1f specifies how to format the code 
#.1 means show 1 digit after the decimal point 
# The f at the end of .1f means format as a floating point number 
print(f"{years:<4}  ${principal:,.2f}")
#The :<4 left aligns the year number in a 4-character field
#The :,.2f Formats the value as currency with commas and the 2 decimal places EX: 1,500.00
print(value, end=" ")
#In Python, end=" " is a parameter used to specify what string should be printed at the end of the output, 
#instead of the default newline character (\n). By default, print() adds a newline after each call, 
#When you set end=" ", it replaces that newline with a space, meaning the next print() output will continue on the same line, separated by a space.
#value: The content to print.
#end: The string appended after value (defaults to "\n").
```
```python
#Default behavior (end="\n")
print("Hello")
print("World")
#Output:
#Hello
#World
#Using end=" "
print("Hello", end=" ")
print("World")
#Output:
#Hello World
```






```python
# This list is going to hold 2 values per slot so leg[1] is going to equal miles[1] and gas[1]  
leg = []
miles = 12
gas = 4
for i in range(2):
  miles += i
  #You can also do something like miles = miles + i
  gas += i
  leg.append((miles, gas))
for i, (miles, gas) in enumerate(leg, 1):
#Pyhton has a enumerate() function with tuple unpacking 
#1 The leg list is a list of tuples, where each tuple contains 2 values (miles, gas)
#Example: leg = [(2.1, 3.2), (4.5, 6.5)]
#2 The enumerate() function goes by enumerate(iterable value, start index) generates pairs of (index value) for each item in the iterable 
#The start parameter "1" sets the starting index because, without it, the starting index would be 0
#Example: (1, (200, 10)) is the first item
        #(2, (300, 12)) is the second item
#3 The for loop unpacks each pair from enumerate() in to two variables, i gets the index 1, 2 ...
```
```python
#This is a simplified version of 
for i in range(len(leg)):
  miles = leg[i][0]
  gas = legs[i][1]
```

```python
#Built in python class functions 
.upper() #iterates over each character and converts input to uppercase 
.isalpha() #ensures only alphabetic characters are processed (ignoring spaces, numbers, symbols, etc)
ord(variable) #gets the ASCII value of whatever input variable 
#(ex: A=65 - Z=90, etc.)
.split() #breaks phrases into a list of words. By default, it splits whitespace. 
#(ex: a variable = "Hello World Hi! 
#variable.split() == ["Hello", "World", "Hi!"])
"".join() #combines into a single string with whatever is in front. In this example, it is nothing joining things without spaces 
#(ex: list = ["H", "e", "l", "l", "o"] 
#joinedVar = "".join(i[0] for i in list) will print out Hello
```
```python
low = -50
high = 50 + 1 #add 1 so it stops at the number you want, for example, if you want 50 you would put 51. it stops 1 number before whatyou put  
increment = 10 
variable = range(low, high, increment)
#variable holds all the numbers between low and high by the increment EX: variable == -50, -40, -30, ... 30, 40, 50
```








```python
#This is the general thing to do compairing things in a while loop, checking stuff and things i will figure out wording later i am very tired loooooool
while True:
  try:
    if compaire != var:
      continue
    else:
      continue
    break
  except ValueError:
    print("Enter a number!")
```
