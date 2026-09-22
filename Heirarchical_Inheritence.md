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
class Details:
    def getName(self):
        self.name = input("Enter name: ")

    def getAge(self):
        self.age = int(input("Enter age: "))


class Employee(Details):
    def getEmployeeDetails(self):
        self.employee_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")


class Patient(Details):
    def getPatientDetails(self):
        self.patient_id = input("Enter patient ID: ")
        self.disease = input("Enter disease: ")


# Employee details
e = Employee()
e.getName()
e.getAge()
e.getEmployeeDetails()

print("\nEmployee Details:")
print("Name:", e.name)
print("Age:", e.age)
print("Employee ID:", e.employee_id)
print("Department:", e.department)


# Patient details
p = Patient()
p.getName()
p.getAge()
p.getPatientDetails()

print("\nPatient Details:")
print("Name:", p.name)
print("Age:", p.age)
print("Patient ID:", p.patient_id)
print("Disease:", p.disease)
```
## Sample Output
<img width="853" height="502" alt="image" src="https://github.com/user-attachments/assets/30a3ef9e-d4b2-42d0-a131-975bebc4223e" />


