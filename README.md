# Bank-Management-System
Bank Management System (Python)

This is a simple console based banking application written in Python.
It allows users to create and manage bank accounts locally using a JSON file for storage.
Each account stores the user's basic information and supports deposit, withdrawal, updates, and deletion.

Features
Option	Function
1	Create a new bank account
2	Deposit money
3	Withdraw money
4	View account details
5	Update account information
6	Delete account
How It Works

When the program starts, it loads data from data.json.

A new account can be created only if the user is 18 or older and provides a 4-digit PIN.

A unique account number is generated automatically.

All changes are saved immediately to data.json.

Sample JSON Database

Below is the stored output saved inside data.json during execution:

[
    {
        "name": "harsh",
        "age": 23,
        "email": "harsh@gmail.com",
        "pin": "1234",
        "account_no": "8Y%tv98",
        "balance": 0
    },
    {
        "name": "Heramb",
        "age": 24,
        "email": "heramb@gmail.com",
        "pin": "1234",
        "account_no": "0Kcl76&",
        "balance": 990000
    }
]

Program Execution Output
press 1 for creating a account
press 2 for Deposite money in the bank
press 3 for Withdrawing money from the bank
press 4 for details
press 5 for updating account details
press 6 for deleting your account
tell your responce:- 1
Enter your name:- Heramb
Enter your age:- 24
Enter your email:- heramb@gmail.com
Enter your pin (4 digits):- 1234
account created successfully
name: Heramb
age: 24
email: heramb@gmail.com
pin: 1234
account_no: 0Kcl76&
balance: 0
please keep your account number safe

tell your responce:- 2
Enter your account number:- 0Kcl76&
Enter your pin:- 1234
Enter amount to deposit:- 1000000
Deposited 1000000. New balance: 1000000

tell your responce:- 3
Enter your account number:- 0Kcl76&
Enter your pin:- 1234
Enter amount to withdraw:- 10000
Withdrew 10000. New balance: 990000

tell your responce:- 4
Enter your account number:- 0Kcl76&
Enter your pin:- 1234
Account details:
name: Heramb
age: 24
email: heramb@gmail.com
pin: 1234
account_no: 0Kcl76&
balance: 990000

How to Run

Install Python

Place main.py and data.json in the same folder

Run the script:

python main.py


Use the menu to perform operations

Notes

Keep your account number and PIN safe as they are required for every transaction.

JSON storage updates after each action so data is preserved even after closing the program.
