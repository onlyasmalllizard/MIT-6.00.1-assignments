# asks the user to think of a number
print("Please think of a number between 0 and 100!")

# initialises values for guess, high, and low
guess = round(99/2)
high = 99
low = 0

while True:
    print("Is your secret number " + str(guess) + "?")
    info = input("Enter 'h' to indicate the guess is too high. Enter 'l' to indicate the guess is too low. Enter 'c' to indicate I guessed correctly. ")
    # if the guess is low, remember that you shouldn't guess below that and make a guess between the current guess and the high point
    if info == 'l':
        low = guess
        guess = guess + round((high - guess)/ 2)
    # if the guess is high, remember that you shouldn't guess above that and make a guess between the current guess and the low point
    elif info == 'h':
        high = guess
        guess = guess - round((guess - low)/ 2)
    # stop guessing because you are correct
    elif info == 'c':
        break

# print the correct guess
print("Game over. Your secret number was: " + str(guess))
