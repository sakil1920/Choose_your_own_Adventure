# Choose_your_own_Adventure

name = input("Type your name: ")
print("Welcome ", name, " to this adventure!")

answer = input(
"You are on a dirt road, it has come to an end and you can go left or right. which way would you like to go? ").lower()

if answer == "left":
answer = input("You come to river, you can walk around it or swim accross? Type walk to walk around and swim to swim accross: ")

    if answer == "swim":
        print("You swim acrross and were eaten by an alligator.")
    elif answer == "walk":
        print("You walked for many miles, ran out of water and you lost the game.")
    else:
        print("Not a valid option. You lose.")

elif answer == "right":
answer = input("You come to a bridge, it looks wobbly, do you want ot cross it or head back (cross/back)? ")

    if answer == "back":
        print("You go back and lose.")
    elif answer == "cross":
        answer = input("You cross the bridge and meet a stranger. Do you talk to them(Yes/No) ")

        if answer == "yes":
            print("you talk to the stanger and they give you gold . you win!")
        elif answer == "no":
            print("you ignore the stranger and they are offended and you lose.")
        else:
            print("Not a valid option. You lose.")
    else:
        print("Not a valid option. You lose.")

print("thank you for trying ", name)
