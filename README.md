# AiCore-Project-documentation 
## AiCore Projects: Milestone Task documentation:
This repository contains milestone task which I have successfully executed and carefully recorded, to serve as form of revision guide to me and also a proof to showcase    my genuine intrest to improve my coding skills with the utimate goal of securing a career in Tech.
Although I am have an Engineering background; I am totally new to python and apart from some self motivated personal learning I have had no previous experiencve in coding with python. I am driven by enthusiasm and genuine passion to learn various software coding packages and hope to study and practice until I am able to comfortably teach others.
I hope you enjoy going through my work.
Thank you.

### Mliestone 3 Task 4
#### Add a section to your README file that explains how you defined the functions you created.
I definined the Functions by ensuring that I observe header . A function header consists of four components:
1. The def keyword
2. The name of the function, following proper naming conventions
3. The optional parameters surrounded by parentheses
4. A colon signifying the end of the function header
### Milestone 4 Task 5
The Hangman class was defined with the init method that took two parameters, word_list and num_lives, with num_lives set to a default value of 5. 

> These attributes listed below were initialized by ensuring parameters are assigned to their corresponding  instance variables 
1.	word: A randomly selected word from the word_list.
2.	word_guessed: A list of underscores ('_') representing the letters of the word that haven't been guessed yet.
3.	num_letters: The number of unique letters in the word.
4.	num_lives: The number of lives the player has at the start of the game. It is the number of incorrect guesses the player is allowed before they lose the game.
5.	word_list: The list of words to choose from. i.e. is a list of words from which the game will randomly select a word for the player to guess
6.	list_of_guesses: A list of letters that have already been guessed.
> Inside the init method, the attributes of the Hangman class are initialized by ensuring, the word_list and num_lives parameters are assigned to instance variables self.word_list and self.num_lives, respectively.
> The random module is used to select a random word from word_list and assign it to the self.word instance variable.
> The self.word_guessed instance variable is initialized as a list of underscores, where the length of the list is equal to the length of self.word ; this  list will be used to display the progress of the player's guesses
> The self.num_letters instance variable is initialized to the number of unique letters in self.word
> Finally, the self.list_of_guesses instance variable is initialized as an empty list, which will be used to keep track of the letters the player has guessed so far.
- The class also includes two methods: check_guess and ask_for_input; to promote name clarity
1.	check_guess: 
The check_guess method takes a guess parameter, converts it to lowercase, and checks if the guess is in the word. If the guess is in the word, it prints a message saying "Good guess! {guess} is in the word." It then updates the word_guessed list to reveal the position of the correctly guessed letter(s) and decrements the num_letters counter. If the guess is not in the word, it decrements the num_lives counter and prints a message saying "Sorry, {guess} is not in the word. You have {self.num_lives} lives left."
2.	ask_for_input: 
The ask_for_input method uses a while loop to keep asking the user to guess a letter until a valid guess is made. It first prompts the user to enter a guess, checks if the guess is a single alphabetical character, and if it has already been guessed. If the guess is not valid, it prints an error message. If the guess is valid, it calls the check_guess method and adds the guess to the list_of_guesses. If the guess is correct, the loop continues until the word is guessed or the player runs out of lives.
