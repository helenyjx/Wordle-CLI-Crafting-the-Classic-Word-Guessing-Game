# Jiaxin-week-11-mini-repo
## Goal
In this demo, I use Rust create a simple game "Wordle", it is a popular online word guessing game, the player is given six attempts to guess a five-letter word chosen by the game's algorithm. After each guess, the game provides feedback on which letters in the guess are correct and in the correct position, which letters are correct but in the wrong position, and which letters are not in the word at all. Using this feedback, the player must guess the correct word before running out of attempts.


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

## eg. my results:
<img width="510" alt="Screen Shot 2023-03-17 at 12 23 52 AM" src="https://user-images.githubusercontent.com/112274822/225812673-01080f57-81a4-44f1-aeb6-c676467be72b.png">
