numberOfGuessesAllowed = 5
numberOfGuessesMade = 0

def check_guess(answer, guess):
    global numberOfGuessesMade
    numberOfGuessesMade += 1
    
    if numberOfGuessesMade > numberOfGuessesAllowed:
        return "You lose!"
    
    if guess == "quit":
        return "Game closed."
    
    guess = int(guess)
    response = ""
    
    if guess > answer:
        response = "Too Big!"
    elif guess < answer:
        response = "Too Small!"
    else:
        return "You win!"

    if abs(guess - answer) <= 5:
        response += " Almost there!"
    elif abs(guess - answer) <= 10:
        response += " Close!"

    return response

# Test cases
answer = 15
test_guesses = [10, 20, 5, 14, 25, "quit"]
for guess in test_guesses:
    print(f"Guess {guess}: {check_guess(answer, guess)}")
