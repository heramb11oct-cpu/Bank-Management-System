# Bank-Management-System

A simple command-line banking application built with Python that allows users to create accounts, deposit/withdraw money, view account details, update information, and delete accounts.

## Features

- **Create Account**: Register a new bank account with personal details
- **Deposit Money**: Add funds to your account
- **Withdraw Money**: Withdraw funds from your account
- **View Details**: Display complete account information
- **Update Account**: Modify account details (name, age, email, pin)
- **Delete Account**: Remove your account from the system

## Requirements

- Python 3.x
- No external dependencies required (uses only standard library)

## Installation

1. Clone or download the repository
2. Ensure `main.py` is in your working directory
3. The application will automatically create a `data.json` file to store account data

## Usage

Run the application using:

```bash
python main.py
```

### Menu Options

When you run the application, you'll see the following menu:

```
press 1 for creating a account
press 2 for Deposite money in the bank
press 3 for Withdrawing money from the bank
press 4 for details
press 5 for updating account details
press 6 for deleting your account
tell your responce:-
```

## Example Usage

### 1. Creating an Account

```
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
```

**Note**: Users must be 18+ years old and PIN must be exactly 4 digits.

### 2. Depositing Money

```
tell your responce:- 2
Enter your account number:- 0Kcl76&
Enter your pin:- 1234
Enter amount to deposit:- 1000000
Deposited 1000000. New balance: 1000000
```

### 3. Withdrawing Money

```
tell your responce:- 3
Enter your account number:- 0Kcl76&
Enter your pin:- 1234
Enter amount to withdraw:- 10000
Withdrew 10000. New balance: 990000
```

### 4. Viewing Account Details

```
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
```

## Data Storage

Account data is stored in `data.json` file. Example structure:

```json
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
```

## Account Number Generation

Account numbers are automatically generated with:
- 3 random letters
- 3 random digits
- 1 special character (!@#$%^&*)
- All shuffled randomly for security

Example: `0Kcl76&`, `8Y%tv98`

## Security Features

- PIN protection for all transactions
- Account number verification required for all operations
- Age verification (must be 18+)
- PIN must be exactly 4 digits

## Validation Rules

- **Age**: Must be 18 or older
- **PIN**: Must be exactly 4 digits
- **Withdrawal**: Cannot exceed available balance
- **Account Operations**: Require both account number and PIN

## Important Notes

⚠️ **Security Warning**: This is a demonstration project. In a production environment:
- Never store PINs in plain text
- Use proper encryption for sensitive data
- Implement secure password hashing
- Add session management and authentication tokens

## File Structure

```
.
├── main.py          # Main application file
└── data.json        # Auto-generated database file
```

## Error Handling

The application handles:
- Missing database file (creates new one)
- Invalid account credentials
- Insufficient balance for withdrawals
- Invalid menu choices
- Database loading errors

## Future Enhancements

- Transfer money between accounts
- Transaction history
- Interest calculation
- Multi-user sessions
- GUI interface
- Password encryption
- Account statements

## Author

Created as a Python learning project for banking system simulation.

## License

This project is open source and available for educational purposes.
