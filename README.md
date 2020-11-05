import random
from time import sleep

choice = ["Rock","Paper","Scissors"]
computer = random.choice(choice)



while player == False:
    print("Welcome to Rock, Paper and Scissors!!")
    print("\nPlease, wait the game is loading.......")
    sleep(3)
    player = input("Which one do you want to choose?\n'Rock':'Rock'\n'Paper'\n'Scissors':'Scissors'\n'Stop the game':'Stop':")
    if player == computer:
        print("\nPlease wait we are loading your results.....")
        sleep(2)
        print("It's a Tie!")
    elif player == "Rock":
        if computer == "Paper":
            print("\nPlease wait we are loading your results.....")
            sleep(2)
            print("You Have Lost!!")
        else:
            print("You Have Won!!")
    elif player == "Scissors":
        if computer == "Rock":
             print("\nPlease wait we are loading your results.....")
             sleep(2)
             print("You Have Lost!!")
        else:
            print("You Have Won!!")
    elif player == "Paper":
        if computer == "Scissors":
            print("\nPlease wait we are loading your results.....")
            sleep(2)
            print("You Have Lost!!")
        else:
            print("You Have Won!!")
    elif player == "Stop":
        print("Thanks for Playing this Game!!")
        break
    else:
        print("That's not a Valid play!!")
        break

    player = False
#By: Bhavana Vankadari

