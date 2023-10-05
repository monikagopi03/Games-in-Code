import random

def play_game():
    user_choice = input("Choose rock, paper, or scissors: ").lower()
    computer_choice = random.choice(["rock", "paper", "scissors"])

    print(f"You chose {user_choice}")
    print(f"The computer chose {computer_choice}")

    if user_choice == computer_choice:
        print("It's a tie!")
    elif user_choice == "rock":
        if computer_choice == "scissors":
            print("You win!")
        else:
            print("Computer wins!")
    elif user_choice == "paper":
        if computer_choice == "rock":
            print("You win!")
        else:
            print("Computer wins!")
    elif user_choice == "scissors":
        if computer_choice == "paper":
            print("You win!")
        else:
            print("Computer wins!")
    else:
        print("Invalid choice. Please choose rock, paper, or scissors.")

while True:
    play_game()
    play_again = input("Do you want to play again? (yes/no): ").lower()
    if play_again != "yes":
        break
        
