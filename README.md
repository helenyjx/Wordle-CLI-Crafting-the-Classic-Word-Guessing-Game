# Jiaxin-week-10-mini-repo
## Goal
In this demo, I use Rust create a simple game "Wordle", it is a popular online word guessing game, the player is given six attempts to guess a five-letter word chosen by the game's algorithm. After each guess, the game provides feedback on which letters in the guess are correct and in the correct position, which letters are correct but in the wrong position, and which letters are not in the word at all. Using this feedback, the player must guess the correct word before running out of attempts.

Overall, this code implements a functional and interactive CLI version of the Wordle game. It demonstrates various Rust features like enums, structs, methods, and modules.

<img width="385" alt="Screen Shot 2023-03-17 at 12 35 52 AM" src="https://user-images.githubusercontent.com/112274822/225813607-cd6ddd91-c01d-4198-80de-5e6adcfe42c9.png">

## Prepration
1. Set virtual environment: 
* `python3 -m venv env`
* `source env/bin/activate`

2. Install rust: 
* `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
* `source "$HOME/.cargo/env"`

3. Create new project:
*  `cargo new src` (src is the project name)

4. After adding main.rs and import words.txt, in terminal, type:
* `cargo run`

## A brief explanation of the code
1. The code starts by importing necessary external libraries, including the colored crate for printing colored text, and the rand crate for generating random numbers. It also defines two custom Rust enums for character matches and attempt results.

2. The Attempt struct represents a single guess attempt by the player. It includes information such as the length of the guess, the guess text, a vector of character match information, and a boolean indicating if the guess was a winning guess. The Attempt struct also has several methods for initializing a new guess, processing a guess, and rendering the guess feedback.

3. The Game struct holds all the game data, including the maximum number of attempts allowed, the list of attempts made, the set of valid words, the length of the target word, and the target word itself. The Game struct also has methods for initializing a new game, making a play (i.e., processing a player guess), and running the game loop.

4. The main function initializes a new Game object and starts the game loop. The loop prompts the player to make a guess and processes the guess by creating a new Attempt object, checking the validity of the guess, rendering feedback, and adding the Attempt to the list of attempts made. If the player guesses the word correctly, the game loop ends and the player wins.

5. The code also includes a tests module with several unit tests for the Attempt struct's methods.

## eg. my results:
<img width="510" alt="Screen Shot 2023-03-17 at 12 23 52 AM" src="https://user-images.githubusercontent.com/112274822/225812673-01080f57-81a4-44f1-aeb6-c676467be72b.png">

### Reference:
1. https://github.com/conradludgate/wordle
2. https://github.com/scottluptowski/wordlet
