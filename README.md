🏦 Bank Operation System (Python OOP)
📘 Overview

This project is a simple Bank Operation System built using Object-Oriented Programming (OOP) in Python.
It allows a user to create an account, deposit money, withdraw money, and view their account balance (mini statement).

🎯 Objectives

Learn and apply basic OOP principles in Python

Create and manage a simple user bank account

Demonstrate use of class, object, methods, and encapsulation

⚙️ Technologies Used

Language: Python 3.x

Environment: Jupyter Notebook (.ipynb)

Concepts Covered:

Class and Object

Instance Variables

Methods

Encapsulation

User Input and Loop Control

💻 Code Explanation
1. Class Definition
class Bank:
    bank_name = "Pragati Life Insurance PLC"
    branch = "Kawran Bazar, Dhaka"


✅ Explanation:
Here, Bank is a class that holds common information for all accounts — such as bank name and branch.

2. Constructor and Attributes
def __init__(self, name, id_no, address):
    self.name = name
    self.id_no = id_no
    self.address = address
    self.balance = 0
    print(f"Hello {self.name}, your account has been created successfully!")


✅ Explanation:
When an account is created, the constructor (__init__) initializes the account holder’s details and sets the initial balance to 0.

3. Deposit Method
def deposit(self, amount):
    self.balance += amount
    print(f"{amount} BDT deposited successfully!")


✅ Adds the given amount to the user’s balance.

4. Withdraw Method
def withdraw(self, amount):
    if amount <= self.balance:
        self.balance -= amount
        print(f"{amount} BDT withdrawn successfully!")
    else:
        print("Sorry! Not enough balance.")


✅ Checks if sufficient balance exists before withdrawal.

5. Mini Statement
def mini_statement(self):
    print(f"Account Holder: {self.name}")
    print(f"Current Balance: {self.balance} BDT")


✅ Displays the account details and current balance.

6. Main Program Loop
while True:
    print("1. Deposit")
    print("2. Withdraw")
    print("3. Mini Statement")
    print("4. Exit")


✅ Keeps running until the user chooses “Exit”.

🧠 Key Learning Points

Class & Object: Used to structure the bank system.

Encapsulation: Balance and user data are stored safely within the class.

Reusability: Same structure can be used to create multiple accounts.

Real-world Application: Mimics actual bank operations in a simple way.

🚀 How to Run

Open the file oop_bank Project.ipynb in Jupyter Notebook or VS Code.

Run all cells in order.

Enter your name, ID, and address.

Choose an option: Deposit, Withdraw, Mini Statement, or Exit.

🏁 Example Output
Welcome to Pragati Life Insurance PLC, Kawran Bazar, Dhaka

Enter your name: Omi
Enter your ID number: 123
Enter your address: Dhaka

Hello Omi, your account has been created successfully!

1. Deposit
2. Withdraw
3. Mini Statement
4. Exit
