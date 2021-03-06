Programming intro


Variables
=========
* Set a value
* Name the value
* Access to it depends on context (location of where it was set) (scope)
```python
 name = "john" 
 num = 25
 
 print(name, num)
```

Arrays []
=========
* Sets one or multiple values to a variable
Example:
```python 
test = [“one”, “two”, “three”] 
```
* Accessing values => test[0] … returns “one”
* Behaves like a box with things in it but those things have no name

Dictionary {}
=========
* Same as a variable but holds multiple variables in one
* Stored as pairs {name : value}
Example => 
```python
test = { "one" : "bike", "two" : "car"}
```
* Accessing values => test[“one”]  … will return “bike”
* Behaves like a box with things in it and those things have names

Functions (def)
=========
* Changes a value
* Takes arguments/parameters
* Optionally returns the new value
* Access to it depends on location it was set (scope)
* Can be used like a variable since it returns a value
```python
def talk(phrase):
    return phrase

print(talk('Hi, world'))
```

Loops (while, for)
==================
* Runs piece of code a given amount of time/depending on condition
* Creates a context (scope)
Example =>
```python
test = [1,2,3,4,5]
for i in test: 
  print(i)
```        
* Creates variable “i” and sets it to each value in the “test” array on each iteration prints the value.
Example => 
```python
test = [1,2,3,4,5]
i=0
while 5 > i:
  print(test[i])
  i+=1
```
* Access to variables depend on scope
* while loops only run until the statement in front of it is true

Classes (object oriented )
==========================
* Allows you to encapsulate code 
* Similar to dictionary and arrays where you name it and access different values
* In order to access the values or function(called methods in classes)  you need to create an “instance” of the class or another name “object”. 
Example => 
```python
class Human: 
  def __init__(self, name):
    self.name = name
    
  def greet(self):
    return f"Hello, my name is {self.name}"
    
 me = Human("Layla")
 print(me.name)
 
```
* returns “layla” and “me” is an object of “Human” class
```python
print(me.greet())
```
* returns 'Hello, my name is Layla' 
* the '\_\_init\_\_' method is a called the "constructor"
* when you first instantiate the object "me" thats the function that is used to set up the object with properties
* "name" is a property of the "me" object
* the "greet" method can access properties in the class
