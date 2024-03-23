# CodSoft_Task-2
import random as r
n=int(input("enter 1 for rock,2 for paper,3 for scissor:"))
L=[1,2,3,4]
L.pop(n)
c=int(r.choice(L))
if n==1:
    print("You chose Rock")
elif n==2:
    print("You chose Paper")
elif n==3:
    print("You chose scissor")
else:
    print("Invalid choice")
if c==1:
    print("Computer chose Rock")
elif c==2:
    print("Computer chose Paper")
elif c==3:
    print("Computer chose Scissor")
else:
    print("Invalid choice")
if((n==1)and(n==3)) or ((n==2)and(c==1)) or ((n==3)and(c==2)):
    print("You win")
elif((n==1)and(c==1)) or ((n==2)and(c==2)) or ((n==3)and(c==3)):
    print("Tie")
else:
    print("You lose")
