# Password Strength Checker

A simple Python program that checks the strength of a password by evaluating its length, the presence of numbers, uppercase letters, and special characters. The program provides feedback and suggestions on how to improve the password strength.

## Features

- **Length Check**: Passwords must be at least 8 characters long.
- **Number Check**: Passwords should contain at least one number.
- **Uppercase Check**: Passwords should contain at least one uppercase letter.
- **Special Character Check**: Passwords should contain at least one special character (e.g., `!@#$%^&*()`).

## Requirements

- Python 3.x

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/username/password-strength-checker.git
---

Feel free to modify and expand on this as needed!

2. **Navigate to home directory**:
   ```bash
   cd password-strength-checker

3. Usage

1. Run the password_strength_checker.py script in your terminal:

```
python password_strength_checker.py
```

2. Enter the password you want to check when prompted.


3. The program will evaluate the password strength and suggest improvements.



Example:

Welcome to Password Strength Checker!
Enter your password: MyPassw0rd!
Strong Password! ✅




How It Works

The script uses regular expressions (regex) to check the following conditions:

Length Check: Password must be at least 8 characters long.

Number Check: Password must contain at least one number.

Uppercase Check: Password must contain at least one uppercase letter.

Special Character Check: Password must contain at least one special character (e.g., !@#$%^&*()).
