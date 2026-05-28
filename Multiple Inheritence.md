# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```
class Add:
    def addition(self, a, b):
        print("Addition:", a + b)

class Sub:
    def subtraction(self, a, b):
        print("Subtraction:", a - b)

class Division(Add, Sub):
    def division(self, a, b):
        print("Division:", a / b)

obj = Division()

x = int(input("Enter first number: "))
y = int(input("Enter second number: "))

obj.addition(x, y)
obj.subtraction(x, y)
obj.division(x, y)
```
## Output Example
```
Enter first number: 20
Enter second number: 5
Addition: 25
Subtraction: 15
Division: 4.0
```
## Result
the output is verified


