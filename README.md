# Use the random numbers to guessing the game
import random

# randint() will generate a random integer between 1-100, assign it to 'number'
number = random.randint(1,100)

# guess will store the guesses that the user makes
guess = 0

# continue the game until the user guesses the answer within 5 attempts
while guess != number:
  guess = int(input("Enter Guess: "))
  # if the user guesses too lower, tell them to guess higher, if they guess
  # too high, tell them to guess lower, and if they get it correct tell
  # them they've won
  if (guess < number):
    print("Guess is too high!")
  elif (guess > number):
    print("Guess is too low!")
  else:
    print("You won!")
#end the game if the user enter the incorrect value upto 5times
#them they've lose
