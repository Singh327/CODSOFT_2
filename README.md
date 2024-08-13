# CODSOFT_2
# Task 2 : Rock, Paper and Scissors game
# Designing rock-paper-scissors GAme with the help of python
import random
# Inputting user's choice
print("Enter your choice :\n 1. Rock\n 2. Paper\n 3. Scissors")
choice= int(input("Enter your choice :"))
if (choice == 1):
    choicename = "Rock"
elif (choice == 2):
    choicename = "Paper"
elif (choice == 3):
    choicename = "Scissors"
else:
    print("Invalid user choice")


# Generating computer's choice
print("Computer's choice\n 1. Rock\n 2. Paper\n 3. Scissors")
comp_choice = random.randint(1,3)
print("Computer's choice is",comp_choice)
if (comp_choice==1):
    comp_choicename = "Rock"
elif (comp_choice==2):
    comp_choicename = "Paper"
elif (comp_choice==3):
    comp_choicename = "Scissors"

#  Logic
print("if it's Rock vs paper , paper wins") 
print("if it's Rock vs Scissors , Rock wins")
print("if it's Scissors vs paper , Scissors wins")


# generating result
print("User's choice is",choicename)
print("Computer's choice is",comp_choicename)
if(choicename == comp_choicename):
    print("It's a tie")
elif (choicename=="Rock" and comp_choicename=="Scissors"):
    print("You win")
elif (choicename == "Paper" and comp_choicename == "Rock"):
    print("You win")
elif (choicename=="Scissors" and comp_choicename=="Paper"):
    print("You win")
else:
    print("Computer wins")
print("Do you want to play another round?")
ans = input("Enter choice: ")
if (ans=="no"):
    print("thanks for playing the game")


