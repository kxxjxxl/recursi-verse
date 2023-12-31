# recursi-verse
crazy concept of recursion - with its potential for infinite loops, if not handled correctly.

The Infinite Loop(s) of Divine Algorithms

This repository contains a collection of classic recursive functions. Recursive functions are functions that call themselves to perform a task, often using a base case to terminate the recursion. In this collection, the base case is when `n = 1`.

Here are 7 examples and exactly 7.

## Table of Contents
1. [Factorial Function](#factorial-function)
2. [Fibonacci Sequence](#fibonacci-sequence)
3. [Sum of an Array](#sum-of-an-array)
4. [Reverse a String](#reverse-a-string)
5. [Greatest Common Divisor (GCD)](#greatest-common-divisor-gcd)
6. [Power Function](#power-function)
7. [Tower of Hanoi](#tower-of-hanoi)

### Factorial Function
Calculates the factorial of a number, which is the product of all positive integers up to that number.
```python
def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n - 1)

```
### Fibonacci Sequence 
Generates the nth number in the Fibonacci sequence, a series where each number is the sum of the two preceding ones.
```python
def fibonacci(n):
    if n == 1:
        return 0
    elif n == 2:
        return 1
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)

```
### Sum Of An Array
Calculates the sum of an array of numbers.
```python
def array_sum(arr):
    if not arr:
        return 0
    else:
        return arr[0] + array_sum(arr[1:])
```
### Reverse A String
Reversing a string using recursion can be a fun exercise.
```python
def reverse_string(s):
    if len(s) <= 1:
        return s
    else:
        return reverse_string(s[1:]) + s[0]

```
### Greatest Common Divisor (GCD)
Finds the greatest common divisor of two numbers.
```python
def gcd(a, b):
    if b == 0:
        return a
    else:
        return gcd(b, a % b)


```
### Power Function
Calculates the power of a number, such as X^n
```python
def power(x, n):
    if n == 1:
        return x
    else:
        return x * power(x, n - 1)



```
### Tower of Hanoi
Calculates the power of a number, such as X^n
```python
def tower_of_hanoi(n, source_peg, target_peg, auxiliary_peg):
    if n == 1:
        print(f"Move disk 1 from {source_peg} to {target_peg}")
        return
    tower_of_hanoi(n - 1, source_peg, auxiliary_peg, target_peg)
    print(f"Move disk {n} from {source_peg} to {target_peg}")
    tower_of_hanoi(n - 1, auxiliary_peg, target_peg, source_peg)


```

# Usage and License
use these functions for whatever you like; they're already out there, after all. these examples are released under a License that you may not yet understand, but you will eventually find it amusing.





