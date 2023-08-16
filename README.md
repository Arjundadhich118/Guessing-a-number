# Guessing-a-number
! A number guessing program is a fun game where the computer thinks of a secret number between a certain range, like 1 to 100. You, the player, try to guess the secret number by entering your guess.

import random

# Generate a random number between 1 and 100
secret_number = random.randint(1, 100)

# Initial number of attempts
num_attempts = 0

# Prompt the user to guess the number
print("Welcome to the Number Guessing Game!")

print("Guess a number between 1 and 100.")

while True:
    guess = int(input("Enter your guess: "))
    num_attempts += 1

    if guess < secret_number:
        print("Too low!")
    elif guess > secret_number:
        print("Too high!")
    else:
        print(f"Congratulations! You guessed the number in {num_attempts} attempts.")
        break
