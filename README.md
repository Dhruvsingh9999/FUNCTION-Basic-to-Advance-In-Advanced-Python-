# FUNCTION-Basic-to-Advance-In-Advanced-Python-
# Functional Programming in Python

## Overview
This repository provides a detailed tutorial on functional programming in Python, including built-in and user-defined functions. It covers the need for functions, their types, arguments, and key concepts such as recursion, decorators, and closures.

## Why Use Functions?
Functions help in structuring and organizing code efficiently. They offer:
- **Reusability**: Code can be reused multiple times without rewriting.
- **Modularity**: Enhances program structure by dividing tasks.
- **Readability**: Improves understanding and maintenance of code.
- **Debugging Efficiency**: Errors can be isolated in functions for easier testing.

## Creating Functions in Python
### Built-in Functions
Python provides several built-in functions like `print()`, `len()`, `type()`, `sum()`, etc.

```python
# Example of a built-in function
str1 = "Hello Python"
print(len(str1))  # Output: 12
```

### User-Defined Functions
User-defined functions are custom functions created by programmers. They can be **parameterized** or **non-parameterized**.

#### 1. Parameterized Functions
Functions that accept parameters and operate on dynamic inputs.

```python
def greet(name):
    print(f"Hello, {name}!")

greet("Dhruv")  # Output: Hello, Dhruv!
```

#### 2. Non-Parameterized Functions
Functions that do not take any parameters.

```python
def display():
    print("Welcome!")
    print("Hello, World!")

display()
```

## Parameters vs. Arguments
- **Parameters**: Variables used in function definitions (formal arguments).
- **Arguments**: Actual values passed to a function when calling it.

```python
def add(a, b):  # Parameters
    return a + b

print(add(5, 10))  # Arguments (Output: 15)
```

## Advanced Concepts
### 1. Nested Functions
A function defined inside another function. Useful for decorators and closures.

```python
def outer_function():
    def inner_function():
        print("Inner function execution")
    inner_function()

outer_function()
```

### 2. Recursion
A function calling itself to solve repetitive problems.

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

### 3. Decorators
A function that modifies another function’s behavior without altering its structure.

```python
def decorator(func):
    def wrapper():
        print("Before function execution")
        func()
        print("After function execution")
    return wrapper

@decorator
def say_hello():
    print("Hello!")

say_hello()
```

## Conclusion
This repository provides a strong foundation in Python functions, covering essential and advanced topics. Functional programming enhances code efficiency, making development easier and more scalable. Explore the provided examples and experiment with writing your own functions!

