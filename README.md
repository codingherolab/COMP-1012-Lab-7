# COMP-1012-Lab-7

Download Here: [COMP 1012: Lab 7](https://codingherolab.com/product/comp-1012-lab-7/)

For Custom/Original Work email codingprolab@gmail.com/whatsapp +1(541)423-7793

Error checking
Read in the file marks.txt. The file format is one number per line. Your program should iterate over all of these numbers, and test to see they they are valid numbers.

Create two lists:

one for valid numbers,
one for invalid numbers.
For a number to be valid, the number:

Must not have any letters inside of it (it must be numeric – use the string function .isnumeric())
Must be greater than or equal to 0
Must be less than or equal to 100
For output, your program should print out the average of the valid inputs, and the list of invalid numbers along with their line number and a reason why they are invalid.

Sample output for data.txt

Average of good data: 45.5

Bad data:

Value ‘4824’ on line 2 is bad because ‘too big’

Value ‘jrfymhnlkt’ on line 3 is bad because ‘not numeric’

Value ‘kvryvqoddj’ on line 4 is bad because ‘not numeric’

Value ‘-95’ on line 6 is bad because ‘not numeric’

…

Hint: Use a tuple to represent cases of invalid data. You can build a tuple using parenthesis:

bad = (1, “shdj”, “not numeric”)  # a tuple!

Hint 2: You can get line numbers by using the enumerate function

Optional: Deduction Game
Write a game where a user has to guess a number from 1 – 99.

Your program will generate a random number once (pick a number), and will then prompts the user to repeatedly guess the number until they get it correct.

During the game, your program will test the number that the user entered compared to the number it picked. If the number that the user guessed is greater than the random number, tell the user “your guess is too low”. If the number that the user guessed is higher than the random number, tell the user, “your guess is too high”. Let the user continue guessing the number generated until they guess it right.

Once the user has successfully guessed the number, tell the user they win, and tell them how many guesses it took them to guess it right.

Use a loop to check your user input. Use string’s .isnumeric() to check to see if the user has provided you with a valid number before you use a cast to an integer. Your program should not crash if the user gives you bad input.

To create a random number use:

import random

myRandomNumber = random.randint(1, 99)

Sample game:

I’ve picked a number between 1 and 99, can you guess it? 50

Nope, it’s not 50

Your guess is too low

I’ve picked a number between 1 and 99, can you guess it? 99

Nope, it’s not 99

Your guess is too high

I’ve picked a number between 1 and 99, can you guess it? 42

Nope, it’s not 42

Your guess is too low

I’ve picked a number between 1 and 99, can you guess it? 93

Nope, it’s not 93

Your guess is too high

I’ve picked a number between 1 and 99, can you guess it? 83

You got it!

It took you 5 guesses.

Optional: New and Improved Deduction Game
Once you’ve completed the guessing game, add some usability improvements. In the line that prompts the user for input, print the known range the random number could be in.

Do not increase the range if the user guesses outside your range. Example, if the current range is 40 to 60, do not change them if the user guesses 100.

Example:

Guess the number. 0 < _ < 100: 50

Guess the number. 0 < _ < 50: 25

Guess the number. 0 < _ < 25: 12

Guess the number. 12 < _ < 25: 18

Guess the number. 12 < _ < 18: 14

Guess the number. 14 < _ < 18: 16

Guess the number. 16 < _ < 18: 17

Congrats you guessed it in 7 tries

Super bonus: What’s the fewest number of guesses you have to make for any range of numbers? Hint: This is a search algorithm called a binary search.
