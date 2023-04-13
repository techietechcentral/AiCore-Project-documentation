# Milestone 1
- To setup a development environment
## Task 1 : setup Github
I successfully setup my development environment and Github account after going through the study content listed below. I am now aware 
of the sercurity key needed to activate activate and link on Github account via bash.
I now know a some important commands I can execute on a VS code git bash terminal to achieve certain opertions e.g
 
```python
[ls] [mkdir] [cd ..] [touch] [rm] [rw-r] [echo] [git init] [git status] [git add] [git rm] [git commit]
[git branch] [git checkout -b] [git checkout] [git merge] [git clone] [vim tutor] [ls-ls] [ls-l] [ls-a]
[conda activate base] [print $PATH] [which ls] [print env] [which python] [echo python $PATH] [python --version]
```
I am now conversant with basic features and capabilities of VS code.
### Prerequisite study content
- What is the command line
- Running terminal commands
- File Manipulation
- The Essentials of Git 
- What is Github?

# Milestone 2 Task 1
- To get comfortable with basic python commands
## Task 1 : Define the list of possible words
### Code
```python
my_first_print = "This print statement was created in Python"
print(my_first_print)
```
```python
age = 38
print("I will be",age, "years old this year")
```
### Task 1 praticals
```python
word_list = ["mango", "orange", "apple", "banana", "grape"]
print(word_list)
```

```python 
A = "A pack of tomatoes"
B = "3 washing sponges"
C = "A litre of juice"
D = "20m of foil"
E = "180g sugar"

A = 0.67
B = 2.70
C = 1.75
D = 3.00
E = 1.10

print("5 packs of tomatoes each costs = £", 5 * A)
print("5 packs of 3 washing sponges each costs = £", 5 * B)
print("5 packs of A litre of juice each costs = £", 5 * C)
print("5 packs of 20m of foil each costs = £", 5 * D)
print("5 packs of 180g sugar each costs = £", 5 * E)
print("Total (without VAT)= £",A + B + C + D + E)
print("Total (with 20% VAT)= £",(0.2 * (A + B + C + D + E) + (A + B + C + D + E)))
print("Round-up Total + 20% VAT)= £",round((0.2 * (A + B + C + D + E) + (A + B + C + D + E)), 2))
```
```python
import decimal
A = decimal.Decimal("0.67")
B = decimal.Decimal("2.70")
C = decimal.Decimal("1.75")
D = decimal.Decimal("3.00")
E = decimal.Decimal("1.15")

print("5 packs of tomatoes each costs = £", 5 * A)
F = 5 * A
print("5 packs of 3 washing sponges each costs = £", 5 * B)
G = 5 * B
print("5 packs of A litre of juice each costs = £", 5 * C)
H = 5 * C
print("5 packs of 20m of foil each costs = £", 5 * D)
I = 5 * D
print("5 packs of 180g sugar each costs = £", 5 * E)
J = 5 * E
total = A + B + C + D + E
print("Total (without VAT) = £",total)
print("Total (with 20% VAT)= £",decimal.Decimal("0.2") * (total) + total)
total_incl_vat = round(decimal.Decimal("0.2") * (total) + (total),2)
print("Round-up Total + 20% VAT)= £",(total_incl_vat))

print("+--------------+-----------------+------------------+-----------------+")
print("|   Quantity   |       Item      |    Unit cost     |    Total cost   |")
print("+--------------+-----------------+------------------+-----------------+")
print("|     5        |pack of Tomaotes |     0.67         |     ", F,"      |")
print("+--------------+-----------------+------------------+-----------------+")
print("|     5        |3x washing sponge|     2.70         |     ", G,"     |")
print("+--------------+-----------------+------------------+-----------------+")
print("|     5        |a litre of juice |     1.75         |     ", H,"      |")
print("+--------------+-----------------+------------------+-----------------+")
print("|     5        |20m foil         |     3.00         |     ", I,"     |")
print("+--------------+-----------------+------------------+-----------------+")
print("|     5        |180g of sugar    |     1.10         |     ", J,"      |")
print("+--------------+-----------------+------------------+-----------------+")
print("|              |            Grand Total(excl VAT)   |     ", total,"      |")
print("+--------------+-----------------+------------------+-----------------+")
print("|              |            Grand Total( + VAT)     |     ", total,"      |")
print("+--------------+-----------------+------------------+-----------------+")
```
```python
h = (25/7)
print (h)
w = (25/2)
print(w)
l = (35)
print(l)
cuboid_volume = (l * w * h)
x = cuboid_volume

cuboid_surface_area = 2*((l*w) + (l*h) + (h*w))
y = cuboid_surface_area
print("The volume of the cuboid is", x, "and it\'s surface area is", round(y,2))

# Cone:
# Height (h): 10
# Radius of base (r): 3
pi = (22/7)
r = 3
h = 10
cone_volume = pi * r**2 * h/3
z = cone_volume

cone_surface_area = pi * r * (r + ((h**2 + r**2)** 0.5))
v = cone_surface_area
print("The volume of cone is", round(z,2), "and the surface area is", round(v,2))
```
```python
import decimal
h = decimal.Decimal(25/7)
print (h)
w = decimal.Decimal(25/2)
print(w)
l = (35)
print(l)
cuboid_volume = decimal.Decimal(l * w * h)
x = cuboid_volume

cuboid_surface_area = 2* decimal.Decimal((l*w) + (l*h) + (h*w))
y = cuboid_surface_area
print("The volume of the cuboid is", round(x,2), "and it\'s surface area is", round(y,2))

# Cone:
# Height (h): 10
# Radius of base (r): 3
pi = (22/7)
r = 3
h = 10
cone_volume = pi * r**2 * h/3
z = cone_volume

cone_surface_area = pi * r * (r + ((h**2 + r**2)** 0.5))
v = cone_surface_area
print("The volume of cone is", round(z,3), "and the surface area is", round(v,3))
```
```python
# Assign variables for each of these items and their prices
# Tomatoes cost 87p for a pack of 6
# 500g sugar costs £1.09
# Washing sponges cost 29p for a pack of 10
# Juice is £1.89 per 1.5l bottle
# Foil is £1.29 per 30m roll
# Using arithmetic operations in Python, calculate the price of 1kg sugar
# What is the price of 20 washing sponges, 3l of juice, and 2 packs of tomatoes?

##Assign variables for each of these items and their prices

k = "2 packs of Tomatoes"
l = "1000g sugar" 
m = "A pack off 20 Washing sponges"
n = "3l bottle Juice"
## Using arithmetic operations in Python, calculate the price of 1kg sugar
print(l, "will cost", (1000 * 1.09)/500,"\n")

# What is the price of 20 washing sponges
print("if", m, "costs", (20 * 0.29)/10)
m = (20 * 0.29)/10
# 3l of juice
print(n, "costs", (3 * 1.89)/1.5)
n = (3 * 1.89)/1.5
# 2 packs of tomatoes?
print("and", k, "costs", (2 * 0.87))
k = (2 * 0.87)
print("Therefore the total price of 20 washing sponges, 3l of juice, and 2 packs of tomatoes will be", (m + n + k)
```
```python
# Car number plate year
# Given the following list of number plates: ["G06 WTR", "WL11 WFL", "QW68 PQR"]
# Extract the last two characters of the first word, which represent the year of the car
# Print the type of each of them
# Convert each of these years to an integer type

nplate_1 = "G06 WTR"
nplate_2 = "WL11 WFL"
nplate_3 = "QW68 PQR"
print(int(nplate_1[1:3]))
print(int(nplate_2[2:4])) 
print(int(nplate_3[2:4]))

type(int(nplate_1[1:3]))
type(int(nplate_2[2:4]))
type(int(nplate_3[2:4]))
```
```python
#BMI Checker
#Given 2 variables, height and weight, calculate the BMI (weight / height ^2).

#Using the parameter BMI, write a series of if statements that print the following outcomes:

#Below 18.5 --> "Your BMI is x. You're in the underweight range."
#Between 18.5 and 24.9 --> "Your BMI is x. You're in the healthy weight range."
#Between 25 and 29.9 --> "Your BMI is x. You're in the overweight range."
#Between 30 and 39.9 --> "Your BMI is x. You're in the obese range."
#Test your code with the following cases by substituting them in for weight and height values in your code:

#Height: 1.83m, Weight: 85kg
#Height: 1.55m, Weight: 61kg
#Height: 2.09m, Weight: 135kg
Height = 2.83
Weight = 850
x = (Weight/(Height**2))

if x <= 18.5:
    print("your BMI is", round(x,2),"you're in the underweight range")
elif (18.5 < x <= 24.9) :
    print("your BMI is", round(x,2), "You're in the healthy weight range")
elif (25 < x <= 29.9) :
    print("your BMI is", round(x,2), "You're in the overweight range")
elif (30 < x <= 39.9) :
    print("your BMI is", round(x,2), "You're in the obese range")
else:
    print("Error")
```
```python
h = input("Enter your Height: ")
h = float(h)
w = input("Enter your Weight: ")
w = float(w)
x = (w/(h**2))
if x <= 18.5:
    print("your BMI is", round(x,2),"you're in the underweight range")
elif 18.5 < x <= 24.9 :
    print("your BMI is", round(x,2), "You're in the healthy weight range")
elif 25 < x <= 29.9 :
    print("your BMI is", round(x,2), "You're in the overweight range")
elif 30 < x <= 39.9 :
    print("your BMI is", round(x,2), "You're in the obese range")
else:
    print("Error...Abnormal result!!\nplease input correct parameters")
```
```python
#Order of Conditions
#Download the next file .
#Run the code and enter 5 as the input. What is the output?
#Run the code again and enter 20 as the input. What is the output?
#Run the code again and enter 50 as the input. What is the output?
#Notice that for all three inputs, you received the same output, why is this?
#Change the order of the conditions so that the correct output is printed for each input

x = int(input('Enter a number: '))
if x > 20: 
    print('x is greater than 20')
elif x > 15:
    print('x is greater than 15')
elif x > 0:
    print('x is greater than 0')
else:
    print('x is less than 0')
```
```python
#Order of Conditions
#Download the next file .
#Run the code and enter 5 as the input. What is the output?
#Run the code again and enter 20 as the input. What is the output?
#Run the code again and enter 50 as the input. What is the output?
#Notice that for all three inputs, you received the same output, why is this?
#Change the order of the conditions so that the correct output is printed for each input

x = int(input('Enter a number: '))
if x > 20: 
    print('x is greater than 20')
elif x > 15:
    print('x is greater than 15')
elif x > 0:
    print('x is greater than 0')
else:
    print('x is less than 0')
```
```pyton
a = 'Altitude'
b = 'airspeed' 
a = 9000
b = 120
if 100 > a or 50000 < a:
    print(a,".ft above ground level is an unsafe flying zone irrespective of airspeed parameter")
elif 60 > b or 500 < b:
    print(b,".knots is an unsafe flying speed; irrespective of Altitude parameter.")
elif (100 <= a or 50000 >= a) and (60 <= b or 500 >= b):
    print(a,".ft and", b,".knots are considered safe flying parameters")
else:
    print('Error')
```
```python
list = ['rock','paper','scissors', '']
#R = 'scissors'
#P = 'paper'
#S = 'scissors'
#list = [R, P, S]

player1 = input('player1 enter rock, paper or scissors: ')
player2 = input('player2 enter rock, paper or scissors: ')

if player1 == list[0] and player2 == list[2]:
    print("player1 wins")
elif player1 == list[2] and player2 == list[0]:
    print("player2 wins")

elif player1 == list[1] and player2 == list[0]:
    print("player1 wins")
elif player1 == list[0] and player2 == list[1]:
    print("player2 wins")

elif player1 == list[2] and player2 == list[1]:
    print("player1 wins")
elif player1 == list[1] and player1 == list[2]:
    print("player2 wins")

elif player1 == list[0] and player2 == list[0]:
    print("it's a tie")
elif player1 == list[1] and player2 == list[1]:
    print("it's a tie")
elif player1 == list[2] and player2 == list[2]:
    print("it's a tie")
    
elif player1 == list[0] and player2 != list[0] or list[1] or list[2]:
    print("Invalid input")
elif player1 == list[1] and player2 != list[0] or list[1] or list[2]:
    print("Invalid input")
elif player1 == list[2] and player2 != list[0] or list[1] or list[2]:
    print("Invalid input")
elif player1 != list[0] and player2 == list[0] or list[1] or list[2]:
    print("Invalid input")
elif player1 != list[1] and player2 == list[0] or list[1] or list[2]:
    print("Invalid input")
elif player1 != list[2] and player2 == list[0] or list[1] or list[2]:
    print("Invalid input")
```
```python
"""task"""

class Sport:
    def __init__(self, type, equipment):   # initialization function
        self.a = type                      # instance variable       
        self.b = equipment                 # instance variable

    def equipment(self):
       print(self.b + ' are very important piece of equipment for '+ self.a)

sport_1 = Sport('climbing','ropes')
sport_1.equipment()
print("==============================================")    
sport_2 = Sport('Skiing','Skis')
sport_2.equipment()
print("==============================================")                   
sport_3 = Sport('sprinting','spike boots')         
sport_3.equipment()
print("==============================================") 
print(sport_1.a)
print(sport_1.b)
print(sport_2.a)
print(sport_2.b)
print(sport_3.a)
print(sport_3.b)
print("---------------------------------------------")   
#print(snow_sport.__dict__)
#print(race_sport.__dict__)

"""task"""
class Sport:
    def __init__(self, type, location, equipment): # function
        self.a = type                      # instance variable
        self.b = location                  # instance variable
        self.c = equipment                 # instance variable
        
    def Equipment(self):
        print(self.a)
        print(self.b)
        print(self.c)
        print("------------------------------------") 
        print(self.a + ' is a good sport')
        print(self.c + ' are very important piece of equipment for '+ self.a)
        print(self.b + ' is the least intresting destination for ' + self.a)
                      
sport_1 = Sport('skiing','France','Skis')
print("*******************************************")
sport_1.Equipment()
print("===========================================")
sport_2 = Sport('Archery', 'Isreal', 'Bow & arrows')
sport_2.Equipment()
```
### Creating a DataFrame From Lists
```python
import pandas as pd
pd. __version__
listPepper = [ 
            [50, "Bell pepper", "Not even spicy"], 
            [5000, "Espelette pepper", "Uncomfortable"], 
            [500000, "Chocolate habanero", "Practically ate pepper spray"]
            ]

dataFrame1 = pd.DataFrame(listPepper)
print(dataFrame1)
```
```python
ds = pd.DataFrame({"Romeo": [95, 28, 32], "Harry": [42, 35,56],"Blake": [11, 22, 39], "Maya": [40, 50, 65],"Hubert": [91, 91, 93], "Jane": [74, 11, 61]})
print(ds)
```
```python
ds = pd.DataFrame({"Romeo": [95, 28, 32], "Harry": [42, 35,56],"Blake": [11, 22, 39], "Maya": [40, 50, 65],"Hubert": [91, 91, 93], "Jane": [74, 11, 61]},index=['1st_mark', '2nd_mark', '3rd_mark'])
print(ds)
```
In connection to milestaone one I have engaged in spending time practicing basic python syntax using VSCode to execute various basic codes involving python operators,
numbers, strings, boolean, creating new files, creating folders incuding the interactive python note book (ipynb) file and the print function. I have learnt quite abit about Lists and and idexing and I found it really intresting.
# Milestone 2 Task 2
- To get comfortable with basic python commands
## Task 2 : Define the list of possible words
To accomplish this task, you will need to use the 'random' module. The random module is one of Python's built-in modules. It has a choice method which returns a random item from a given sequence.
Step 1. Go to the first line of your file.
Step 2. Write import random on the line. Note: To import a module, you have to use the import keyword at the top of the file.
Step 3: Create the random.choice method and pass the word_list variable into the choice method.
Step 4: Assign the randomly generated word to a variable called word.
Step 5: Print out word to the standard output. Run the code several times and observe the words printed out after each run.
```python
mylist = ["yellow", "blue", "car", "green", "wine", "goods", "weather", "safety"]
#print(dir(random))

import random
random.choice(mylist)
word = random.choice(mylist)
print(word)
```
### Prerequisite study content
- Numbers
- Strings
- Editing files with nano
- Running Python files from the terminal
- A tour of VSCode
- The VSCode integrated terminal
- Markdown
- Python files and Python Notebooks
- What is Python
- How (and how not) to run Python files from VSCode
- Printing things in Python
- Variables
- Booleans
- Lists
# Milestone 2
- To get comfortable with basic python commands
## Task 3 and 4 : Ask user for input and check input is single chartacter
```python
guess = input("Please enter a single Character: ")

if  guess.isalpha() == True and len(guess) == 1:
    print("Good guess!")
elif  guess.isalpha() == False and len(guess) == 1:
    print("invalid input... Please Enter a single Character")         
else:
    print("Oops! That is not a valid input.")
```
At the end of milestaone 2 I have consolidated my knowledge of milestone subjects and I  am now conversant with writing codes and opening terminals in VScode. I have also practiced coding in python where have learnt about the following 
- function
- import
- __init__
- dictionary
- tuple
- List
- set
- if, elif, and else statement 

### Milestone 3 Task 1
- Check if the guessed character is in the word
- In this milestone I will check if the guessed letter is in the radomly chosen word.
Write code that will continuously ask the user for a letter and validate it.
Create a new script called milestone_3.py. This file will contain the code for this milestone.
Step 1. Create a while loop and set the condition to True. Setting the condition to True ensures that the code run continuously.
In the body of the loop, write the code required for the following steps.
Step 2: Ask the user to guess a letter and assign this to a variable called guess.
Step 3. Check that the guess is a single, alphabetical character.
Step 4. If the guess passes the checks, break out of the loop.
Step 5: If the guess does not pass the checks, then print a message saying "Invalid letter. Please, enter a single alphabetical character."
```python

'''
while True:
    guess = input('Please, enter a single alphabetical character :')
    if guess.isalpha() == True and len(guess) == 1 and guess != int:
        break
    else:
        print("Invalid letter. Please, enter a single alphabetical character.")
   ```
    
### Milestone 3 Task 2
- Iteratively check if the input is a valid guess
Check whether the letter guessed by the user is in the secret word that was randomly chosen by the computer. For example, if the user guesses the letter "a" and the secret word is "apple", then your code should check if "a" is in "apple".
Step 1. Create an if statement that checks if the guess is in the word.
Step 2. In the body of the if statement, print a message saying "Good guess! {guess} is in the word.". Obviously, format the string to show the actual guess instead of {guess}.
Step 3. Create an else block that prints a message saying "Sorry, {guess} is not in the word. Try again." This block of code will run if the guess is not in the word.

```python

'''Rev 3.2 - Check whether the letter guessed by the user is in the secret word that was 
randomly chosen by the computer (capital excluded)'''
mylist = ["blue", "car", 'horse', 'titanium', 'composite']
import random
random.choice(mylist)
word = random.choice(mylist)
print(f'{word} is the radom word in question')

guess = input('Please, enter a single alphabetical character: ')
while guess == guess in word:
    if len(guess) == 0:
        guess = input('Please, enter a single alphabetical character: ')
    elif (len(guess) == 1) and guess.isalpha() == True:
        print(f'Good guess! {guess} is in {word}.')
        break    
else:
    print(f'Sorry, {guess} is not in {word}. Try again.')
    ```

```python
'''Rev 3.4 - this function Checks whether the letter guessed by the user is in the secret word that was 
randomly chosen by the computer (Milestone 3 task 2). 
Capital Letters have now been introduced as valid inputs in this version'''

mylist = ["blue", "car", 'horse', 'titanium', 'composite']

def check_guess(): 
    import random
    random.choice(mylist)
    word = random.choice(mylist)
    print(f'{word} is the radom word in question')

    guess = (input('Please, enter a single alphabetical character: ')).lower()
    while guess == guess in word:
        if len(guess) == 0:
            guess = input('Please, enter a single alphabetical character: ').lower()
        elif (len(guess) == 1) and guess.isalpha() == True:
            print(f'Good guess! {guess} is in {word}.')
            break    # this controls the loop depending on indent
    else:
        print(f'Sorry, {guess} is not in {word}. Try again.')
check_guess()
```
### Milestone 3 Task 3
- check whether the guess is in the word.

Good job so far! But your code probably doesn't look great. It's hard to tell which lines do what.
Create 2 functions, check_guess and ask_for_input functions which contain the code for those two things.
The check_guess function will take the guessed letter as an argument and check if the letter is in the word.
Step 1: Define a function called check_guess. pass in the guess as a parameter for the function. Write the code for the following steps in the body of this function.
Step 2: Convert the guess into lower case.
Step 3. Move the code that you wrote to check if the guess is in the word into this function block.
The ask_for_input function.
Step 1. Define a function called ask_for_input.
Step 2. Move the code that you wrote in the Iteratively check if the input is a valid guess task into this function block.
Step 3. Outside the while loop, but within this function, call the check_guess function to check if the guess is in the word. Don't forget to pass in the guess as an argument to the method.
Step 4. Outside the function, call the ask_for_input function to test your code.

```python
'''Rev 3.5 - this function Checks whether the letter guessed by the user is in the secret word that was 
randomly chosen by the computer (Milestone 3 task 2). 
Capital Letters have now been introduced as valid inputs in this version'''

mylist = ["blue", "car", 'horse', 'titanium', 'composite']

def ask_for_input():
    while True:
        guess = (input('Please, enter a single alphabetical character :')).lower()
        if guess.isalpha() == True and len(guess) == 1 and guess != int:
            print("correct! valid input")   
            break
        else:
            print("Invalid letter. Please, enter a single alphabetical character.")
check_guess()
ask_for_input()
```
#### ***Milestone 4***
```python
mylist = ["blue", "car", 'horse', 'titanium', 'composite']

def check_guess(): 
    import random
    random.choice(mylist)
    word = random.choice(mylist)
    print(f'{word} is the radom word in question')

    guess = (input('Please, enter a single alphabetical character: ')).lower()
    while guess == guess in word:
        if len(guess) == 0:
            guess = input('Please, enter a single alphabetical character: ').lower()
        elif (len(guess) == 1) and guess.isalpha() == True:
            print(f'Good guess! {guess} is in {word}.')
            break    # this controls the loop depending on indent
    else:
        print(f'Sorry, {guess} is not in {word}. Try again.')
check_guess()
```
> - Create a new script called milestone_4.py. This file will contain the code for the third milestone.
Define the init method of the Hangman class.
- Step 1. Create a class called Hangman.
- Step 2. Inside the class, create an init method to initialise the attributes of the class. Pass in word_list and num_lives as parameters. Make num_lives a default parameter and set the value to 5.
- Step 3. Initialise the following attributes:
1. word: The word to be guessed, picked randomly from the word_list. ***Remember to import the random module into your script.***
2. word_guessed: list - A list of the letters of the word, with for each letter not yet guessed. For example, if the word is 'apple', the word_guessed list would be ['', '', '', '', '']. If the player guesses 'a', the list would be ['a', '', '', '', ''].
3. num_letters: int - The number of UNIQUE letters in the word that have not been guessed yet.
4. num_lives: int - The number of lives the player has at the start of the game.
5. word_list: list - A list of words.
6. list_of_guesses: list - A list of the guesses that have already been tried. Set this to an empty list initially.
```python
# import the random module
import random
# Step 1. Create a class called Hangman.
class Hangman:
    #Inside the class, create an init method to initialise the attributes of the class. 
    # Pass in word_list and num_lives as parameters. 
    # Make num_lives a default parameter and set the value to 5.
    def __init__(self, word_list, num_lives=5):
        # Initialise the following attributes:
        self.word_list = word_list  
        self.num_lives = num_lives  # num_lives: int - The number of lives the player has at the start of the game.
        self.word = random.choice(word_list)    # word: The word to be guessed
        self.word_guessed = ['' for _ in range(len(self.word))]     # word_guessed: list - A list of the letters of the word, with for each letter not yet guessed
        self.num_letters = len(set(self.word))  # num_letters: int - The number of UNIQUE letters in the word that have not been guessed yet
        self.list_of_guesses = []   # list_of_guesses: list - A list of the guesses that have already been tried. Set this to an empty list initially.
```
```python
'''
In the code below, we import the random module and define the Hangman class. 
The __init__ method initializes the attributes of the class. 
It takes in word_list and num_lives as parameters. 
num_lives is a default parameter and its value is set to 5.

We initialize the word_list and num_lives attributes with the values passed in as parameters. 
Then, we randomly select a word from the word_list using the random.choice() method 
and store it in the word attribute.

We also initialize the word_guessed attribute to a list of empty strings with a length equal
to the length of the word. This list will keep track of the letters in the word that have 
not yet been guessed. We initialize num_letters to the number of unique letters in the word.

Finally, we initialize the list_of_guesses attribute to an empty list. This list will keep 
track of the letters that have already been guessed.
'''

import random

class Hangman:
    def __init__(self, word_list, num_lives=5):
        self.word_list = word_list
        self.num_lives = num_lives
        self.word = random.choice(word_list)
        self.word_guessed = ['' for _ in range(len(self.word))]
        self.num_letters = len(set(self.word))
        self.list_of_guesses = []
```
```python
class Hangman:
    def __init__(self, word_list, num_lives=5):
        self.word_list = word_list
        self.num_lives = num_lives
        self.word = random.choice(word_list)
        self.word_guessed = ['_' for _ in range(len(self.word))]
        self.num_letters = len(set(self.word))
        self.list_of_guesses = []

    def check_guess(self, guess):
        guess = guess.lower()
        if guess in self.word:
            print(f"Good guess! {guess} is in the word.")
            for i in range(len(self.word)):
                if self.word[i] == guess:
                    self.word_guessed[i] = guess
            self.num_letters -= 1
        else:
            self.num_lives -= 1
        print(f"Sorry, {guess} is not in the word.")
        print(f"You have {self.num_lives} lives left.")

    def ask_for_input(self):
        while True:
            guess = input("Guess a letter: ")
            if len(guess) != 1 or not guess.isalpha():
                print("Invalid letter. Please, enter a single alphabetical character.")
            elif guess in self.list_of_guesses:
                print("You already tried that letter!")
            else:
                self.check_guess(guess)
                self.list_of_guesses.append(guess)
                break
```

```python
import random

class Hangman:
    """
    A class representing a game of Hangman.

    Attributes:
    - word_list (list): A list of words to choose from for the game.
    - num_lives (int): The number of lives the player has to guess the word.
    - word (str): The word chosen for the game.
    - word_guessed (list): A list of underscores representing the letters of the word to guess.
    - num_letters (int): The number of unique letters in the word to guess.
    - list_of_guesses (list): A list of letters guessed by the player.

    Methods:
    - __init__(self, word_list, num_lives=5): Initializes the Hangman game with the given word list and number of lives.
    - check_guess(self, guess): Checks if the guessed letter is in the word, updates the word_guessed list if necessary,
      and decrements the number of lives if the guess is incorrect.
    - ask_for_input(self): Prompts the player to enter a letter guess and handles invalid input.
    """

    def __init__(self, word_list, num_lives=5):
        """
        Initializes the Hangman game with the given word list and number of lives.

        Args:
        - word_list (list): A list of words to choose from for the game.
        - num_lives (int): The number of lives the player has to guess the word.
        """
        self.word_list = word_list
        self.num_lives = num_lives
        self.word = random.choice(word_list)
        self.word_guessed = ['_' for _ in range(len(self.word))]
        self.num_letters = len(set(self.word))
        self.list_of_guesses = []

    def check_guess(self, guess):
        """
        Checks if the guessed letter is in the word, updates the word_guessed list if necessary,
        and decrements the number of lives if the guess is incorrect.

        Args:
        - guess (str): The letter guessed by the player.
        """
        guess = guess.lower()
        if guess in self.word:
            print(f"Good guess! {guess} is in the word.")
            for i in range(len(self.word)):
                if self.word[i] == guess:
                    self.word_guessed[i] = guess
            self.num_letters -= 1
        else:
            self.num_lives -= 1
        print(f"Sorry, {guess} is not in the word.")
        print(f"You have {self.num_lives} lives left.")

    def ask_for_input(self):
        """
        Prompts the player to enter a letter guess and handles invalid input.
        """
        while True:
            guess = input("Guess a letter: ")
            if len(guess) != 1 or not guess.isalpha():
                print("Invalid letter. Please, enter a single alphabetical character.")
            elif guess in self.list_of_guesses:
                print("You already tried that letter!")
            else:
                self.check_guess(guess)
                self.list_of_guesses.append(guess)
                break
```          
