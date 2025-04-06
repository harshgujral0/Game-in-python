import random
choices=["rock","paper","scissor"]
while True:
 user_choice=input("Enter your choice(rock,paper,scissor)").lower()
 computer_choice=random.choice(choices)
 print("Computer choose:",computer_choice)
 if user_choice == computer_choice:
    print("Its a Tie!")
 elif user_choice=="rock":
    if computer_choice=="scissor":
        print("You Win Rock crusher Scissor")
    else:
        print("You Loose! Paper covers Rock")
 elif user_choice=="paper":
    if computer_choice=="rock":
        print("You Win! Paper cover rocks")
    else:
        print("You Loose! Scissor Cut Paper")
 elif user_choice=="scissor":
    if computer_choice=="paper":
        print("You Win! Scissor Cuts Paper")
    else:
        print("You Loose! Rock crushes Scissor")
 else:
    print("Invalid Input. Please choose rock paper or scissor")       

 play_again=input("Do you want to play again").lower()
 if play_again!="yes":
     print('Thanks for Playing!')
     break
