# Rock-paper-scissor

import random
def user_computer(user,system):
    if user==computer:
        print("It's a TIE")
    else:
        if ((user=="rock" and system=="scissor") or\
            (user=="scissor" and system=="paper") or\
            (user=="paper" and system=="rock")):
            print("User WON")
        else:
            print("System WON")
def user_user2(user,user2):
    if user==user2:
        print("It's a TIE")
    else:
        if ((user=="rock" and user2=="scissor") or\
            (user=="scissor" and user2=="paper") or\
            (user=="paper" and user2=="rock")):
            print("User1 WON")
        else:
            print("user2 WON")
input_type=input("Choose System or User: ")
input_type=input_type.lower()
user=input("Enter input: ")
games=["rock","paper","scissor"]
if input_type=="system":
    computer=random.choice(games)
    print("System choice: "+computer)
    user_computer(user,computer)
else:
    user2=input("Enter input: ")
    if user2 in games:
        user_user2(user,user2)
    else:
        print("Enter valid input")
