# assi2
import random
name=input("what is your name? ")
print("All the Best",name)
colour = 
["red","orange","blue","green","yellow","white","black","violet","silver","golden","brown","pink","p
urple","grey"]
word=random.choice(colour);
print("Guess the characters in colour:")
guesses=''
turn=6
while turn>0:
 count=0
 for char in word:
 if char in guesses:
 print(char)
 else:
 print("---")
 count +=1
 if count == 0:
 print("congratulations............you are winner",name)
 print("the colour is",word)
 break
 guess=input("guess a character in country:")
 guesses += guess
 if guess not in word:
 turn -= 1
 print("sorry!.....you are worng guess")
 print("you have",+ turn,'more guesses:')
 if turn == 0:
 print("you loose......Sorry")
output:
what is your name? Rameshwari
All the Best rameshwari
Guess the characters in colour:
---
---
---
---
---
---
guess a character in country:o

o
---
---
---
---
---
guess a character in country:g
o
---
---
---
g
---
guess a character in country:p
sorry!.....you are worng guess
you have 5 more guesses:
o
---
---
---
g
---
guess a character in country:r
o
r
---
---
g
---
guess a character in country:n
o
r
---
n
g
---
guess a character in country:e
o
r
---
n
g
e
guess a character in country:a
o
r
a
n
g
e
congratulations............you are winner rameshwari
the colour is orange
