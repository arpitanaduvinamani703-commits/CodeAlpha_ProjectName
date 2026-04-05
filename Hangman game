import random

# List of words
words = ["python", "computer", "program", "internship", "network"]

word = random.choice(words)
guessed_letters = []
attempts = 6
display = ["_"] * len(word)

print("Welcome to Hangman Game!")

while attempts > 0 and "_" in display:
    print("\nWord:", " ".join(display))
    guess = input("Enter a letter: ").lower()

    if guess in guessed_letters:
        print("You already guessed that letter.")
        continue

    guessed_letters.append(guess)

    if guess in word:
        for i in range(len(word)):
            if word[i] == guess:
                display[i] = guess
        print("Correct guess!")
    else:
        attempts -= 1
        print("Wrong guess! Attempts left:", attempts)

if "_" not in display:
    print("\nCongratulations! You guessed the word:", word)
else:
    print("\nGame Over! The word was:", word)
