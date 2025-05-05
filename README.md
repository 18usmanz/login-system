# Login System

This is a simple Python-based login and signup system that uses file handling to store user credentials securely by hashing passwords.

## Features
- **User Registration (Signup)**
  - New users can create accounts by providing an email and password.
  - Passwords are hashed using SHA-256 before being stored.

- **User Login**
  - Existing users can log in by entering their email and password.
  - Passwords are checked by comparing the stored hash.

- **Account Locking**
  - After 3 failed login attempts, an account is automatically locked and cannot log in again unless manually unlocked.

- **Secure Password Input**
  - Passwords are hidden (masked) during input using `pwinput`.

## How It Works
- User credentials are stored in `credentials.txt` as `email hashed_password`.
- Locked accounts are listed in `locked.txt`.

## Requirements
- Python 3.x
- `pwinput` package (for hidden password input)

Install `pwinput` via pip if you don't have it:
```bash
pip install pwinput
