# strengthen_password_generater
Password Strength Checker
password = input("Enter password: ")

if len(password) < 6:
    print("Weak password")
elif any(char.isdigit() for char in password) and any(not char.isalnum() for char in password):
    print("Strong password")
else:
    print("Medium password")

