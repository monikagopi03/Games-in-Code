import random

# Generate a random number between 1 and 100
secret_number = random.randint(1, 100)

# Initialize the number of tries
attempts = 0

print("Welcome to the Guessing Game!")
print("I'm thinking of a number between 1 and 100.")

while True:
    # Ask the player for a guess
    guess = int(input("Enter your guess: "))
    
    # Increase the number of attempts
    attempts += 1
    
    # Check if the guess is correct
    if guess == secret_number:
        print(f"Congratulations! You guessed the number in {attempts} attempts.")
        break
    elif guess < secret_number:
        print("Too low. Try again.")
    else:
        print("Too high. Try again.")
        
