import time

def space():
    for rep in range(2):
        print("")

print(''''*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
******************************************************************************''')

print("")
print("{:^80}".format("\033[4:36m Welcome to Treasure Island \033[m"))
print("")
print("Your mission is to find  the treasure.")
choice_one = str(input("You're at a cross road. Where do you want to go? [Left] or [Right] ")).title()

print("")
process = "P", "R", "O", "C", "E", "S", "S", "I", "N", "G", ".", ".", "."
print("")

for loading in process:
    print(f'\033[1:32m{loading}\033[m', end=" ", flush=True)
    time.sleep(0.3)

if choice_one == "Right":
    space()
    print("\033[1:31mFall into a hole.\n"
          "Game Over\033[m")

elif choice_one != "Left":
    space()
    print("\033[1:31mFall into a hole.\n"
          "Game Over\033[m")

elif choice_one == "Left":
    print("")
    space()

    choice_two = str(input("You've come to a lake. There is an island in the middle of the lake. Type [Wait] to wait for a boat. Type [Swim] to swim across. ")).title()

    print("")
    process = "P", "R", "O", "C", "E", "S", "S", "I", "N", "G", ".", ".", "."
    print("")

    for loading in process:
        print(f'\033[1:32m{loading}\033[m', end=" ", flush=True)
        time.sleep(0.3)

    if choice_two == "Swim":
        space()
        print("\033[1:31mAttacked by trout\n"
            "Game Over\033[m")

    elif choice_two != "Wait":
        space()
        print("\033[1:31mAttacked by trout\n"
              "Game Over\033[m")

    elif choice_two == "Wait":
        print("")
        space()

        choice_three = str(input("You arrive at the island unharmed. There is a house with 3 doors. One [Red], one [Yellow] and one [Blue]. Which colour do you choose? ")).title()

        print("")
        process = "P", "R", "O", "C", "E", "S", "S", "I", "N", "G", ".", ".", "."
        print("")

        for loading in process:
            print(f'\033[1:32m{loading}\033[m', end=" ", flush=True)
            time.sleep(0.3)

        if choice_three == "Red":
            space()
            print("\033[1:31mBurned by fire.\n"
            "Game Over\033[m")

        elif choice_three == "Blue":
            space()
            print("\033[1:31mEaten by beasts.\n"
            "Game Over\033[m")

        elif choice_three != "Yellow":
            space()
            print("\033[1:31mGame Over\033[m")

        elif choice_three == "Yellow":
            print("")
            space()
            print("\033[1:32mYou found the treasure!\n"
            "You Win!\033[m")

print("")
print("                      \033[7:31m --> FINISHED SYSTEM <--\033[m")
