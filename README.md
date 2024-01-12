# PasswordGenerator

import random
import string

def generate_password(length=12):
    # Define characters for the password
    characters = string.ascii_letters + string.digits + string.punctuation

    # Generate a random password using the defined characters
    password = ''.join(random.choice(characters) for _ in range(length))

    return password

def main():
    # Specify the desired password length (default is 12)
    password_length = 16

    # Generate a password
    password = generate_password(password_length)

    # Print the generated password
    print("Generated Password:")
    print(password)

if __name__ == "__main__":
    main()
