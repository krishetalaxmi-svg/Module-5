# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program

    # Get user input
    name = input("Enter student name: ")
    
    # Define the class
    class Student:
        # Default constructor
        def __init__(self):
            self.a = name   # assign input to instance variable
    
        # Method to display message
        def show(self):
            print("This is non-parameterized constructor")
            print("Welcome", self.a)
    
    # Create object
    s = Student()
    
    # Call method
    s.show()

## Output
<img width="691" height="359" alt="image" src="https://github.com/user-attachments/assets/387fb62e-ff99-42ac-9433-14ff2e1c6be8" />

## Result
The program was executed successfully. A Student class with a default (non-parameterized) constructor was created, and it correctly displayed a welcome message
using the user-provided name.

# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
      class Demo:
          
      
          def __init__(self):
              self.status = "Alive"
              print(self.status)
          
      
          def __del__(self):
              print("Object is being destroyed")
      
      
      obj = Demo()
      
      
      del obj

## 🧪 Output
<img width="657" height="386" alt="image" src="https://github.com/user-attachments/assets/d235e797-0952-4b47-b442-eb5731598271" />

## Result
The program was executed successfully. A class with a constructor and destructor was implemented, where the constructor initializes and displays the status, and the destructor is automatically invoked when the object is deleted

