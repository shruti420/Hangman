# Hangman

This file contains classic hangmen.In our program, computer will be player one and the person guessing will be player two.

First, you create a function called _hangmen_ to store the game.
The function accepts a variable called _word_ as a parameter, which is the word player to has to guess. The variable wrong keeps track of player two's incorrect guesses.
Stages is a list of strings when Python prints each stage in the stages list on a new line, a picture of a hangman forms.The variable remaining letters is a list containing each character in the variable word, it keeps track of which letters are left to guess.
The variable _board_ is a list of strings, you use it to keep track of the game board you display to player two, for example, if the word is cat and play or two has already correctly guessed C and T.
This code populates the board list with an underscore for every character in a variable word.

The program also has a _wind_ variable that starts as false to keep track of weather player to has won the game yet finally you print.

The next part of code is a loop that keeps the game going, your loop continues as long as the variable wrong is less than the length of the stages list, minus one. This means the game will continue until player two has guessed more wrong letters than the number of strings it takes to create the hangmen. We have to subtract one from the length of the stages list to compensate for the fact that the stages list starts counting from zero and wrong starts counting at one. Once we are inside your loop, we print a blank space to make the game look nice when it prints in the shell, then you collect player 2's guess and save it in the variable char.

Next,we can check to see if player two guessed correctly by seeing if their guess is in the list of remaining letters. If player two guessed correctly, you need to update your board list, for example, if player two guests see, you would need to update board list to look like this. Pythons index function returns the index, the first occurrence of a character in a list to update your board, you use the index function to find the first occurrence of the letter player to guest in the list remaining letters.

We then use that index to replace the corresponding underscore in the board list with the letter they guessed. You replace the letter they guessed with a dollar sign so that the letter player to guest is no longer in the remaining letters list, replacing the letter with a character like a dollar sign is easier than removing it from the list. If player two guesses incorrectly, you simply increment the variable wrong by one.

Next, you call the join method on a space and pass the variable board, which prints out the board so player two can see it and use it to make their next guests. Now it is time to print the hangman, to print your hangmen at whatever stage the game is that you have to slice your stage's list. You start at stage zero and slice up to the stage you are at, represented by the variable wrong plus one. You add one because when you are slicing the end slice does not get included in the result. Slicing from zero to the integer stored in the variable wrong plus one gives you the strings you need to print the hangman at whatever stage the game is at.

Finally, you check if there are any more underscores left in the board list, if there aren't, it means player to successfully guessed every letter in the word and won the game. One player, two wins, you print you in, then you print the board. One last time, set the variable win to true and break out of the loop. Once you break out of your loop, if player to one you do nothing, the program is over.
If they lost, the variable win is false. If that is the case, you print the full hangmen and you lose followed by the word they couldn't guess.

Here is your complete code.


