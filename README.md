# Snowman, a command line JavaScript application

## 1. Running this application

* `git clone` this repo.
* Open up the app in VSCode or a similar IDE.
* run `npm install` to install any dependencies this project uses.
* run `npm install chalk` to install chalk.
* run `node snowman.js` and have some fun.

## 2. Dependencies

`require` package is used in this application to read in user input.

```npm install require```

```javacript
const chalk = require('chalk')
const readline = require('readline-sync')
```

## 3. Game Structure

Check the game structure in this `Trello`  [board](https://trello.com/b/QqA9QRFZ/snowman) 

### Snowman control flow

* The computer pick a word at random from a library
* The user should see a number of `_` characters equal to the number of letters in the word (ex. B _ _ C _ _ N, for `bitcoin`)

#### The user is able to enter guesses

* Invalid guesses are handled by displaying a message and having the user enter a different guess. Invalid guesses don't count against the guess count.
* After each guess, the user sees the new updated word, replacing all _ with letters they have guessed
* After each guess, the user sees the letters they have guessed already
* After each incorrect guess, the number of guesses decreases.
* After each correct guess, the number of guesses stays the same.

#### The user knows how many guesses are left

* At the beginning of the game, the number of guesses remaining are visible
* After each guess, the updated number of guesses are visible

#### The user is able to see the correct answer regardless winning or losing

* The game continues until the user has won or lost
* Once the full word is guessed, the game displays how many guesses it took and displays a victory message
* If the user runs out of guesses, the full word is revealed and the game displays a defeat message

## 4. Snowman

![Snowman-Game](./snowman.gif)


## Bonus Features

If cloning this repo or working on the Snowman implementation, please feel free to add additional Snowman features like being able to enter the word for a last chance if the user has only 1 guess left.  

