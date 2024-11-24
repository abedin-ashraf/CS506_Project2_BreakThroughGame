# BreakthroughGame

BreakthroughGame is an implementation of the classic abstract strategy board game **Breakthrough**, invented by Dan Troyka in 2000. This project features intelligent agents that play the game using Minimax search, Alpha-Beta pruning, and configurable heuristics for offensive and defensive strategies.

---

## Table of Contents
- [About the Game](#about-the-game)
- [Features](#features)
- [Installation](#installation)
- [How to Play](#how-to-play)
- [Project Structure](#project-structure)
- [Configuration Options](#configuration-options)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## About the Game
Breakthrough is a two-player zero-sum board game played on an 8x8 grid where each player controls 16 workers. The objective is to:
1. Move one of your workers to the opponent's base (the last row).
2. Or capture all opponent workers.

### Rules:
- Workers move **one square forward** or **diagonally forward**.
- Workers capture opponent pieces only by **diagonal forward moves**.
- A worker cannot jump over another piece.

This project implements intelligent agents that use AI algorithms to play the game optimally.

---

## Features
1. **AI Agents**:
   - Minimax Agent.
   - Alpha-Beta Pruning Agent.
2. **Heuristic Evaluation Functions**:
   - Offensive: Focused on capturing opponent pieces and advancing toward the goal.
   - Defensive: Focused on preserving one's pieces and blocking opponent movement.
3. **Extended Rules**:
   - Play on a 5x10 rectangular board.
   - Win condition requiring 3 workers to reach the opponent's base.

4. **Configurable**: Adjust depth, heuristics, and playstyle (offensive/defensive) for agents.

---

## Installation

### Prerequisites
- Python 3.6 or later.
- `pygame` library.

### Steps
1. Clone the repository or download the ZIP file.
   ```bash
   git clone <repository_url>
   cd BreakthroughGame
   ```
2. Install dependencies:
   ```bash
   pip install pygame
   ```

---

## How to Play

1. Open the project in an IDE like PyCharm, VS Code, or any Python editor.
2. Run the `breakthroughgame.py` script:
   ```bash
   python breakthroughgame.py
   ```
3. Follow on-screen instructions to:
   - Play the game as Player 1 or Player 2.
   - Let the AI agents compete against each other.

For extended rules, run the `breakthroughgame_extend.py` file:
```bash
python breakthroughgame_extend.py
```

---

## Project Structure
```
BreakthroughGame/
├── alpha_beta_agent.py       # Alpha-Beta pruning agent implementation
├── breakthroughgame.py       # Main game script
├── breakthroughgame_extend.py# Game script with extended rules
├── example.py                # Example scenarios and usage
├── minimax_agent.py          # Minimax agent implementation
├── model.py                  # Game state and mechanics
├── src/                      # Supporting files for gameplay
├── README.md                 # Project documentation
└── requirements.txt          # List of dependencies
```

---

## Configuration Options
Customize the following parameters in the `breakthroughgame.py` file to experiment with agent behavior:
1. **Depth of Search**: Adjust how far the agent searches.
2. **Heuristics**: Switch between offensive and defensive strategies.
3. **Board Size**: Change the board to 5x10 for extended rules.

---

## Future Enhancements
- **Graphical User Interface**:
  - Add a GUI to enhance interactivity.
- **Reinforcement Learning**:
  - Implement an agent that learns and adapts from games played.
- **Multiplayer Support**:
  - Enable online multiplayer functionality.
- **Dynamic Heuristics**:
  - Incorporate adaptive heuristics that evolve with the state of the game.

---

## License
This project was developed as part of an academic assignment for CS 591. For inquiries, contact the contributors.