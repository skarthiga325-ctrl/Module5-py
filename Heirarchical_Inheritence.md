# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```
class Person:
    def get_name(self):
        self.name = input("Enter name: ")

class Employee(Person):
    def get_employee(self):
        self.emp_id = input("Enter employee id: ")

    def display_employee(self):
        print("Employee Name:", self.name)
        print("Employee ID:", self.emp_id)

class Patient(Person):
    def get_patient(self):
        self.patient_id = input("Enter patient id: ")

    def display_patient(self):
        print("Patient Name:", self.name)
        print("Patient ID:", self.patient_id)

e = Employee()
e.get_name()
e.get_employee()
e.display_employee()

p = Patient()
p.get_name()
p.get_patient()
p.display_patient()
```
## Sample Output
```
Enter name: Arun
Enter employee id: E101
Employee Name: Arun
Employee ID: E101

Enter name: Meena
Enter patient id: P201
Patient Name: Meena
Patient ID: P201
```

## Result
the output is verified




