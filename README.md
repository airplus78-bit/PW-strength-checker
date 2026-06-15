# PW-strength-checker
def check_password(password):
    if len(password) < 8:
        return "Weak (too short)"
    elif password.isdigit():
        return "Weak (numbers only)"
    elif password.isalpha():
        return "Weak (letters only)"
    else:
        return "Strong password"

pw = input("Enter a password: ")
print(check_password(pw))
