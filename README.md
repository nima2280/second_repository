# second_repository
import random
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

print("Welcome to the Password Generator!")
az_letters= int(input("How many letters would you like in your password?\n"))
az_symbols = int(input(f"How many symbols would you like?\n"))
az_numbers = int(input(f"How many numbers would you like?\n"))

def password_generator(az_letters, az_symbols, az_numbers):
  password = ' '
  for i in range(az_letters):
    password += random.choice(letters)
    print(i)
  for i in range(az_symbols):
      password += random.choice(symbols)
    print(i)
  for i in range(az_numbers):
    password += random.choice(numbers)
    print(i)
 
