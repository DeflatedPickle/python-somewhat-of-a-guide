# Functions

## What is a Function?

A function is a command that can be used to perform an/or multiple actions. They can contain however many lines of code you would like, and can be used however many times by just calling it.

### Why Should I Use Functions?

Using functions will decrease the the amount of coding needed.

If you want to run multiple lines of code multiple times, then putting that code into a function will reduce the lines needed to 1 - the function call. It also means that you can update the code you want to run, easily, rather than having to change a line in each duplicate section of code.

## Arguments {#arguments}

### What is an Argument?

An argument is something that can be passed into a function to then be used inside of the function.

```python
def greet(name):
    print("Hello, " + name + "!")
```

```python
def greet_long(first_name, second_name):
    print("Hello, " + first_name + " " + second_name + "!")
```

This will print, "Hello, Monty Python!".

### Default Value

By default, the values of arguments are all empty, and so every one must have a value passed to it. However, you might want to give default values for arguments. This can be done by adding an equals sign and then the value, just like you were creating a variable.

```python
def greet(name="Monty"):
    print("Hello, " + name + "!")
```

### Passing Arguments

To pass values to function arguments, you will need to add the data to the set of parentheses.

```python
greet("Monty")
```

If there are multiple arguments for a function, to set their values, you will need to set them in the order they come in the function.

You can also pass the name of the argument and then it's value.

```python
greet(name="Monty")
```

Passing them with the name means that you can give the values anywhere in the parentheses.

```python
greet_long(second_name="Python", first_name="Monty")
```

These aren't an either/or situation, though. Both can be used together.

```python
greet_long("Monty", second_name="Python")
```

However, you can't pass a named argument and then an unnamed one, as the order of the arguments does matter.

```python
greet_long(second_name="Python", "Monty")
```

Using the name of the argument will improve readability of the code, and if you think someone else will need to understand what the arguments mean, it might be a good idea to use them.

### What are Args and Kwargs?

When making a function, you can specify that in the arguments, it can accept either only `*args` or a number of arguments and then `*args`. What `*args` means, is a limitless amount of arguments, so creating a function that accepts it, means that all arguments provided to the call after specific ones, will be placed in a list called: "`args`". You can then access the arguments as `args` in the function to use them.

```python
def function(*args):
    for item in args:
        print(item)

function("Hello", "World!")
```

You can also, after `*args` \(if used\), ask for `**kwagrs`. What `**kwargs` means, is a limitless amount of keyword arguments. It's essentially the same as `*args`, though it only accepts named arguments, and the named arguments will be placed in a dictionary as key/value pairs, called: "`kwargs`".

```python
def function(**kwargs):
	for k, v in kwargs.items():
		print(v)

function(first="Hello", second="World!")
```

##  Returning Information {#returning-information}

Functions can return information to be used elsewhere.

```python
def sum(num1, num2):
    return num1 + num2

print(sum(1, 2))
```

This function will add the 2 arguments together.

## Generators

### What is a Generator?

## Decorators {#coroutines}

### What is a Decorator?

