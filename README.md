# Minesweeper AI

Minesweeper is a puzzle game where the objective is to clear a board containing hidden "mines" without detonating any of them. The AI developed in this project uses logical reasoning to safely identify and flag all the mines on the board.

## Table of Contents
- [Description](#description)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Functions](#functions)
- [Outcomes](#outcomes)
- [License](#license)

## Description
Designed and developed an AI agent to play the classic Minesweeper game using propositional logic and knowledge representation. The AI can infer safe cells and mines based on the game's rules and logical sentences, aiming to flag all mines and avoid detonating them.

## Technologies Used
- Python
- Propositional Logic
- Artificial Intelligence
- Game Development

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/minesweeper.git
    ```
2. Navigate to the project directory:
    ```sh
    cd minesweeper
    ```
3. Ensure you have Python 3.11 installed. If not, download and install it from [Python's official website](https://www.python.org/downloads/).
4. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage
1. To start the game, run:
    ```sh
    python runner.py
    ```
2. Observe the AI making moves and solving the Minesweeper board.

## Project Structure
- `runner.py`: Contains the code to run the graphical interface for the game.
- `minesweeper.py`: Contains all of the logic for playing the game and making optimal moves.
- `requirements.txt`: Contains the list of packages required for the project.

## Functions

### Sentence Class
- **known_mines()**: Returns a set of all cells known to be mines.
- **known_safes()**: Returns a set of all cells known to be safe.
- **mark_mine(cell)**: Updates the sentence if cell is known to be a mine.
- **mark_safe(cell)**: Updates the sentence if cell is known to be safe.

### MinesweeperAI Class
- **add_knowledge(cell, count)**: Updates the AI's knowledge base with new information about `cell`.
- **make_safe_move()**: Returns a move that is known to be safe.
- **make_random_move()**: Returns a random move if no safe move is possible.

## Outcomes
Successfully implemented an AI capable of playing Minesweeper by making informed decisions based on logical inferences, demonstrating advanced problem-solving skills and knowledge in artificial intelligence.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
