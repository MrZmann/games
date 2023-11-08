For this assignment, you will get to implement a game of your choice and then present your work to the class.

You can either choose two projects from the first group or one project from the second group. (You are welcome to do more though!)
You could also choose one project from the third group. Projects in this group are very challenging so if you choose one of these you can work with up to one other partner if you would like to.

### First Group:

- Quiz Game
- Mad Libs
- Guess my Number
- Smart Rock Paper Scissors

### Second Group:

- Quiz Game (with at least 3 extra credit options)
- Pass the Pig
- Hangman
- Wordle

### Third Group:

- Pass the Pig (with at least 3 extra credit options)
- Connect 4
- Any game from the above groups if you send an email summary at the end (https://mailtrap.io/blog/python-send-email/)

Finally, if there is a different game / project / extra credit task you would be interested in, just ask me!

## Deadlines:

- Nov 9, 11:59 PM - Choose your game(s). You must submit some code (push to your repo). This will count as your attendance for Thursday.
- Nov 13, 11:59 PM - if you chose two games from the first group, one must be finished (pushed to the repo) by Monday night. Everyone else should be about halfway done. Create a file called status.txt and write what you have done so far and any questions that you have. Push this file before midnight.
- Nov 15, 2:00 PM - Presentations

## Quiz Game

Ask the user at least 10 questions of your choice. Each question should have at least four answer choices (a, b, c, d). Exactly one answer choice should be correct for each question. After each response, you should print if it was correct or not. At the end of the game you should print the overall score.

Requirements:

- Case shouldn't matter (if the user answers A or a, those are both the same)
- If the user gives invalid input, you should keep asking for a valid answer choice until it is valid
- At the end of the game, ask the user if they want to play again

Extra Credit:

- Shuffle the questions and answer choices. If you take the quiz again, the answers choices will show up in a different order, the questions will also be reordered.
- Add a time limit. Give the user only a few seconds to answer before moving on to the next question. You might have to do something [like this](https://stackoverflow.com/questions/1335507/keyboard-input-with-timeout)
- Keep a leaderboard. Ask the user for their name and then store their score. After each game, print the leaderboard (sorted by score).
- Store the leaderboard in a file so when you start up the game again you can see the old leaderboard
- Make it pretty (you can use emojis, ascii art, or [colors](https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal))

## Mad Libs

Mad libs is a funny game where you ask the user for various words, and then use those words to fill in a story.

Try it out [here](https://www.thepaintedturtle.org/sites/main/files/file-attachments/mad_libs.pdf)

Requirements:

- For this game, you must ask the user for at least 15 words. At the end, print out the whole story.
- If the user presses enter before typing a word, re-prompt them for the same word

Extra Credit:

- Ask the user if they want to save their story to a file. If they do, ask them what they want the file to be called.

## Guess my Number

Pick a number between 1 and 10000 (hint: random.randint()). Repeatedly ask the user to guess. If the guess is too low, print it is too low. If it is too high, print it is too high. If they get it right, congratulate the user and tell them how many guesses it took.

Requirements:

- If the user inputs a number outside of the range, or if they input something that is not an integer, re-prompt the user for a valid response.

Extra Credit:

- Keep a leaderboard. Ask the user for their name and then store their score. After each game, print the leaderboard (sorted by score).
- Store the leaderboard in a file so when you start up the game again you can see the old leaderboard
- Make it pretty (you can use emojis, ascii art, or [colors](https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal))

## Smart Rock Paper Scissors

When you start a game of rock paper scissors, ask the player what game mode they would like to play. For Game Mode = 1, the computer will play randomly. For Game Mode = 2, ask the user what percentage of the time they would like to win (1-100). Hint - use random.randint(?, ?), what are the odds that number will be larger than the percent of the time the user wants to win?

Requirements:

- If the user provides invalid input, re-prompt
- Once the round is over ask if the user wants to play again
- Keep score and print out the number of wins, number of draws, number of losses at the end of each round

## Pass the Pig

In this game, you can roll a die (random.randint or random.choice). If you roll a 1, your turn is over and you don't get any points. If you roll a 2-6, you get that many points for the round and you also get the opportunity to roll again. If you roll again, you might lose it all (if you roll a 1), but you might also score more points. If you choose to end your turn, the next player can play.

Example Gameplay:

Round 1:
- Player one rolls 2, 4 --> 6 points
- Player two rolls 2, 3, end turn --> 5 points

Round 2:
- Player one rolls 3, 2, 5, 1 --> 6 + no points --> 6 points
- Player two rolls 6, 2, end turn --> 5 + 8 --> 13 points

Requirements:

- Must support 2-6 players (everyone will take turns at the same keyboard)
- Must print whose turn it is at the beginning of each turn, along with the score of both players
- Re-prompt in case of invalid inputs
- First player to 100 points wins

Extra Credit:

- Support for bots with different strategies. Each strategy should be written in its own function. One example strategy might be to always end after 5 rolls. Create at least 3 unique strategies.
- Support for bot only mode (print the end result at least). Run your bots against themselves. Each game should finish very fast. Which strategy wins the most on average?
- At the end of the game, graph each player's score over time using matplotlib
- Print some [pig ascii art](https://ascii.co.uk/art/pig)

## Hangman

Choose a five letter word.

The user will guess a letter. If the letter is not in the word they lose one life. After each guess print out the word (using underscores for the letters they haven't discovered yet).

After 8 wrong guesses, the user loses and you can print out the answer.

Extra Credit:

- Choose a random 5 letter word from a list
- Choose a random 5 letter word from a file like [this one](https://gist.github.com/cfreshman/a03ef2cba789d8cf00c08f767e0fad7b).
- Create a leaderboard

## Wordle

This game is strictly harder to code than Hangman is, but you should still try if you like it!
Choose a five letter word.

The user will guess a five letter word. For each letter, let the user know if that letter was either:

- not in the word
- in the word at this position
- in the word at another position

They will have 6 guesses. If they get the word right, they win. If they don't get it in 6 guesses, they lose and you print the word.

Extra Credit:

- Choose a random 5 letter word from a list
- Choose a random 5 letter word from a file like [this one](https://gist.github.com/cfreshman/a03ef2cba789d8cf00c08f767e0fad7b).
- Print pretty output (you can use emojis, ascii art, or [colors](https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal))

## Connect 4

https://stackoverflow.com/questions/1335507/keyboard-input-with-timeout
You should have a board with 7 columns and 6 rows. There are two players. Each turn one player can select a column (re-prompt if the column is invalid or full). By selecting that column, they place a piece at the bottom-most empty space in that column (loop through that column from bottom to top and place it in the first free space). When a piece is placed you should check if it makes four in a row horizontally or vertically. If it does, that player wins, if not the game goes on until someone wins or the board fills up.

Requirements:

- After each turn, print the board state. Empty spaces can be represented as \_, Player 1 can be X, Player 2 can be O. Feel free to change how it looks though.

Extra Credit:

- Allow players to win by getting 4 in a row diagonally
- Allow for a variably sized board
- Make it pretty (you can use emojis, ascii art, or [colors](https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal))
