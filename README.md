# Guessing-a-number
! A number guessing program is a fun game where the computer thinks of a secret number between a certain range, like 1 to 100. You, the player, try to guess the secret number by entering your guess.

import random

def guess_number():
     secret_number = random.randint(1, 100)
    attempts = 0

    while True:
        guess = int(input("Guess a number between 1 and 100: "))
        attempts += 1

        if guess < secret_number:
            print("Try a higher number.")
        elif guess > secret_number:
            print("Try a lower number.")
        else:
            print(f"Congratulations! You guessed the number {secret_number} in {attempts} attempts.")
            break

guess_number()
