# 2048 Game

A fully functional implementation of the classic **2048 puzzle game**, built with vanilla JavaScript. The goal is to slide numbered tiles on a 4×4 grid and combine them to reach the 2048 tile!

## Live Preview
**Live Demo:** [Play the game here](https://seemsgood78.github.io/2048-game/)

## How to Play
- Use **arrow keys** (←↑→↓) to slide all tiles in a direction
- When two tiles with the **same number** collide, they merge into one
- After each move, a new **2** (90% chance) or **4** (10% chance) appears in a random empty cell
- Reach the **2048 tile** to win!
- The game is over when **no moves are available**

## Features
* **Core Game Logic:** All movement, merging, and scoring logic encapsulated in a clean `Game` class module.
* **Keyboard Controls:** Smooth tile movement using arrow key events.
* **Score Tracking:** Score increases by the sum of all merged tiles per move.
* **Win & Game Over Detection:** Displays messages when 2048 is reached or no moves remain.
* **Restart Functionality:** Reset the game to its initial state at any time.

## Technologies Used 💻

**Core**
* **HTML5** — Semantic markup.
* **CSS3** — Pre-written styles with dynamic cell classes (`field-cell--{value}`).
* **JavaScript (ES6+)** — Game logic via an exported `Game` class.

**Development & Deployment**
* **Vite** — Fast build tool and development server.
* **GitHub Pages** — Hosting and deployment.

## Getting Started

Follow these instructions to set up the project locally:

1. **Clone the repository:**
```bash
git clone https://github.com/SeemsGood78/2048-game.git
cd 2048-game
```

2. **Install dependencies:**
```bash
npm install
```

3. **Run the project locally:**
```bash
npm run start
```

## Game Class API

| Method | Description |
|---|---|
| `constructor(initialState?)` | Creates a new game, optional initial board state |
| `getState()` | Returns the current 4×4 board |
| `getScore()` | Returns the current score |
| `getStatus()` | Returns `idle`, `playing`, `win`, or `lose` |
| `moveLeft()` | Slides all tiles left |
| `moveRight()` | Slides all tiles right |
| `moveUp()` | Slides all tiles up |
| `moveDown()` | Slides all tiles down |
| `start()` | Starts the game |
| `restart()` | Resets the game to its initial state |
