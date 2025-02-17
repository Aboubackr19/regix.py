import re  # Import the re module to work with regular expressions

# Function to validate email
def validate_email(email):
    pattern = r"^[a-z0-9]+[._]?[a-z0-9]+@[a-z0-9]+\.[a-z]{2,3}$"
    return bool(re.match(pattern, email))

# Function to validate phone number
def validate_phone_number(phone_number):
    pattern = r"^(\(\d{3}\)\s?|\d{3}[-\s]?)\d{3}[-\s]?\d{4}$"
    return bool(re.match(pattern, phone_number))

# Function to validate password security
def validate_password(password):
    pattern = r"^(?=.*[A-Z])(?=.*[a-z])(?=.*\d)(?=.*[@#$%^&+=!]).{8,}$"
    return bool(re.match(pattern, password))

# Example inputs for testing
emails = ["aboubackrdiouf@gmail.com", "abou_doe@domain.co", "diouf123@domain.corporate", "@gmail.com"]
phone_numbers = ["314-498-5607", "(314) 498-5607", "314 498 5607", "(314)-498-5607", "3144985607", "123.456.7890", "123-45-7890"]
passwords = ["Abcd1234!", "weakpass", "STRONGpass1$", "NoSpecial123"]

# Running validation tests
for email in emails:
    print(f"{email}: {validate_email(email)}")  # Expected output: True True False False

for number in phone_numbers:
    print(f"{number}: {validate_phone_number(number)}")  # Expected output: True True True True True False False

for password in passwords:
    print(f"{password}: {validate_password(password)}")  # Expected output: True False True False
