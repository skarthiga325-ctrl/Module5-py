# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```
class Person:
    def get_name(self):
        self.name = input("Enter name: ")

class Details(Person):
    def get_age(self):
        self.age = int(input("Enter age: "))

class Location(Details):
    def get_location(self):
        self.place = input("Enter location: ")

    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)
        print("Location:", self.place)

obj = Location()
obj.get_name()
obj.get_age()
obj.get_location()
obj.display()
```

## Sample Output
```
Enter name: Arun
Enter age: 21
Enter location: Chennai
Name: Arun
Age: 21
Location: Chennai
```
## Result
the output is verified

