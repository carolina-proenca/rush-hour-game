# rush-hour-game
Project developed as part of the Artificial Intelligence and Data Science course in the second semester of the 2023/2024 academic year.

Rush Hour Game

Rush Hour is a logic game in which the objective is to move the red car to the exit, located in the last two positions of the row where it is located. To do this, you will need to move the other vehicles on the board to clear the way.

Game Rules

  - The board is a square grid (currently only levels for 6x6 grids have been defined).
  - Vehicles can occupy 2 or 3 squares and be oriented vertically or horizontally.
  - Vertical vehicles can only move up and down.
  - Horizontal vehicles can only move left and right.
  - No vehicle can go beyond the limits of the board or cross other vehicles.

Features

  - Textual interface and graphical interface.
  - Selection of levels with different configurations and difficulties.
  - Possibility to watch the game being solved automatically by search algorithms.
  - Manual game mode, with the option to ask for a hint.
    
Search Algorithms Implemented

Search algorithms were used to solve the different levels:

Uninformed search:

  - Breadth-First Search (BFS)
  - Depth-First Search (DFS)

Informed search:

  - A*
  - Greedy Search

Informed searches use two different heuristics:

  - Manhattan distance between the red car and the exit.
  - Number of vehicles directly blocking the red car's path.

Requirements

  - Python 3
  - Libraries: pygame, sys

How to use the text interface

  - Access the terminal in the Game directory.
  - Run the command: python3 rush_hour_terminal.py

Available options:

  - Learn the rules of the game.
  - Manually play any of the 10 available levels.
  - Watch a search algorithm solve a level.
  - During manual play, you can ask for a single hint by pressing the H key.

Game control:

  - Select the letter corresponding to the vehicle you want to move.
  - Then choose the direction of movement.
  - Empty spaces are represented by *.
  - The red car is represented by the letter X.

How to use the graphical interface

  - Install the pygame library (if not already installed).
  - In the Game directory, run: python3 rush_hour_graphical_interface.py

In the main menu:

  - Select “Rules” to review the game rules.
  - Select “Play” to choose the difficulty level: Easy (level 3), Medium (level 6), Hard (level 10)
  - The game will be solved automatically using the Breadth-First Search algorithm.
