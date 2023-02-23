# Hangman
Hangman is a classic game in which a player thinks of a word and the other player tries to guess that word within a certain amount of attempts.

This is an implementation of the Hangman game, where the computer thinks of a word and the user tries to guess it. 

For milestone 2: Create the variables for game
Task 1: Define list of possible words
1. print list of fruits
Task 2: Choose a random word from list using random module
2. select random fruit
Task 3: Ask user for an alphabet input
3. ask user to input an alphabet
Task 4: Check if input is a valid single alphabet character
4. check if input is valid

For milestone 3:
Create 2 functions, check_guess and ask_for_input functions which contain the code for those two things.
function `ask_for_input`:
- does step 3 - 4 in milestone 2
- Additionally convert the letter to lowercase
- Call the function Check 'check_guess' that checks the guess of the word is in the letter or not

function `check_guess`:
The check_guess function will take the guessed letter as an argument and check if the letter is in the word.

Milestone 4: Create the Game class (mileston_4.py) `Hangman`
Attribues:
- word: The word to be guessed, picked randomly from the word_list. 
- word_guessed: list - A list of the letters of the word, with _ for each letter not yet guessed. For example, if the word is 'apple', the word_guessed list would be ['_', '_', '_', '_', '_']. If the player guesses 'a', the list would be ['a', '_', '_', '_', '_'].
- num_letters: int - The number of UNIQUE letters in the word that have not been guessed yet.
- num_lives: int - The number of lives the player has at the start of the game.
- word_list: list - A list of words.
- list_of_guesses: list - A list of the guesses that have already been tried. Set this to an empty list initially.

Methods:
`check_guess` method:
- convert guess to lower case
- if guess in word then in the `if` block, replace the corresponding "_" in the `word_guessed` with the guess.
- else if not in word then reduce `num_lives` by 1

`ask_for_input` method:
- ask user to input a single alphabet