# 💣 Minesweeper AI Game

**Introduction to Artificial Intelligence with Python**  
📍 *Granville, OH | November 2023 – December 2023*

## 🧠 Overview

This project implements a logic-based AI agent to play the classic **Minesweeper** game using **propositional logic**, **subset inference**, and a **dynamic knowledge base**. The AI simulates human reasoning: from marking safe cells to flagging mines, deducing new facts and playing interactively through a GUI built with **Pygame**.

The result is an intelligent system capable of solving Minesweeper boards while visualizing the reasoning process in real time.

---

## ✨ Features

- 🧠 **Knowledge-Based AI**
  - Uses logical sentences to represent board knowledge
  - Applies **subset inference** to deduce safe cells and mines
  - Updates its belief system dynamically based on new information

- 🎮 **Interactive GUI (Pygame)**
  - Click to reveal cells or flag mines
  - Press **"AI Move"** to let the agent make its best move
  - Press **"Reset"** to start a new game
  - Full visual rendering of flags, mines, numbers, and game status

- 📚 **Reasoning Logic Highlights**
  - Builds knowledge using `Sentence(cell_set, mine_count)`
  - Identifies and marks known mines and safes
  - Infers new knowledge by comparing logical subsets (e.g., if A ⊂ B, then B−A must have count−A.count mines)

---

## 🗂️ Project Structure

- `minesweeper.py`  
  Core game logic, including:
  - `Minesweeper` class for board generation and rules
  - `Sentence` class for propositional logic representation
  - `MinesweeperAI` class for knowledge-based reasoning

- `runner.py`  
  Pygame GUI for interactive play, with buttons for AI move, reset, and user interactions.

- `assets/`  
  Static assets for GUI rendering
  - `fonts/`
    - `OpenSans-Regular.ttf` — font for text display
  - `images/`
    - `flag.png` — icon for flagged cells  
    - `mine.png` — icon for revealed mines

- `README.md`  
  Project documentation




---

## 🏁 How to Run

### Requirements

- Python 3.x  
- Pygame (`pip install pygame`)

### Run the Game

```bash
git clone https://github.com/yourusername/minesweeper-ai.git
cd minesweeper-ai
pip install pygame
python runner.py


