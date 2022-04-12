# snake-water-gun-game
I'm writing this code for exercise while learning python.
import random
a = ["snake" , "water" , "gun"]

i=1
v=0
print("let's start the game")
while(i<=10) :
    b = random.choice(a)
    c = str(input("enter water , snake or gun"))
    i+=1
    if c == "snake" :
        if b == "water" :
            print("you won")
            v+=1
        else :
            print("you lost")
    elif c == "water" :
        if b == "gun" :
            print("you won")
            v+=1
        else :
            print("you lost")
    elif c == "gun" :
        if b == "snake" :
            print("you won")
            v+=1
        else :
            print("you lost")
print("you won",v,"times")
print("computer won",10-v,"times")
