# Password-Strength-Checker
import re

def check_password_strength(password):
    strength = 0

    # Check password length
    if len(password) >= 8:
        strength += 1
    else:
        print("- Password is too short. Use at least 8 characters.")

    # Check for numbers
    if re.search(r"\d", password):
        strength += 1
    else:
        print("- Add numbers to your password.")

    # Check for uppercase letters
    if re.search(r"[A-Z]", password):
        strength += 1
    else:
        print("- Add uppercase letters to your password.")

    # Check for special characters
    if re.search(r"[!@#$%^&*(),.?\":{}|<>]", password):
        strength += 1
    else:
        print("- Add special characters to your password.")

    # Final strength evaluation
    if strength == 4:
        print("Strong Password! ✅")
    elif strength == 3:
        print("Moderately Strong Password. Consider making it stronger.")
    else:
        print("Weak Password. ⚠️ Improve it based on the above suggestions.")

if __name__ == "__main__":
    print("Welcome to Password Strength Checker!")
    user_password = input("Enter your password: ")
    check_password_strength(user_password)
