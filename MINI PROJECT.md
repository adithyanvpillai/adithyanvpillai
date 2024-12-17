import random
i=0
c=5
number=random.randint(1,100)
guess=0

print("*** WELCOME TO THE NUMBER GUESSING GAME ***")
print(" ")
print("Guess a number between 1 to 100")
print(" ")
      
while i<c:
    print(c-i,'try left')
    guess=int(input("Enter your Guess: "))
    if guess>100 :
        print("Guess a number between 1-100")
    elif guess<number :
        print("Guess Higher!!")
    elif guess>number :
        print("Guess Lower!!")
    elif guess==number:
        print("🎉 Congratulations! You guessed the number ",number)
        break
    i+=1
    if i==5:
        print(“GAME OVER!! ”,number,”was the number”)
