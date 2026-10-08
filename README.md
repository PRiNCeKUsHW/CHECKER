# Connect Four (CHECKER)

A two-player **Connect Four** game that runs in the browser, built with HTML, CSS and jQuery.

## Features

- Two players enter their names at the start (Player 1 is **blue**, Player 2 is **red**)
- Click a column and your chip drops to the lowest empty slot
- Detects horizontal, vertical and diagonal wins of four in a row
- Shows whose turn it is, and announces the winner when the game ends (refresh to play again)

## Tech Stack

- HTML5
- CSS3
- JavaScript + jQuery

## How to Run

No build step or server is needed.

```bash
git clone https://github.com/PRiNCeKUsHW/CHECKER.git
cd CHECKER
```

Then open `index.html` in any modern browser.

## Project Structure

```
CHECKER/
├── index.html   # Game board (6 x 7 grid of buttons)
├── proj1.css    # Board and chip styling
└── proj2.js     # Game logic: turns, chip drop, win checks
```

## How It Works

- `checkBottom(col)` finds the lowest gray cell in the clicked column.
- `horizontalWinCheck()`, `verticalWinCheck()` and `diagonalWinCheck()` scan the board after every move.
- Turns alternate between the two players until someone connects four.
