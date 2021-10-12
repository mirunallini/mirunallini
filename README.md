import random

user_action = input("Enter a choice (rock, paper, scissors): ")
possible_actions = ["rock", "paper", "scissors"]
computer_action = random.choice(possible_actions)
print(f"\nYou chose {user_action}, computer chose {computer_action}.\n")

if user_action == computer_action:
    print(f"Both players selected {user_action}. It's a tie!")
elif user_action == "rock":
    if computer_action == "scissors":
        print("Rock smashes scissors! ,user gain 1 point")
    else:
        print("Paper covers rock!,user lose 1 point")
elif user_action == "paper":
    if computer_action == "rock":
        print("Paper covers rock!,user gain 1 point")
    else:
        print("Scissors cuts paper!,user lose 1 point")
elif user_action == "scissors":
    if computer_action == "paper":
        print("Scissors cuts paper! ,user gain 1 point")
    else:
        print("Rock smashes scissors! ,user lose 1 point")
