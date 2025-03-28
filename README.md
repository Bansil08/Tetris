# 🎮Tetris Game

A classic Tetris game implementation in C++ for Windows consoles, featuring colorful blocks, multiple difficulty levels, a hold piece mechanic, and a scoring system. Built with standard C++ libraries and Windows-specific console functions for rendering and input handling.

## ✨Features
- **Tetrominoes**: Standard 7 shapes (I, O, T, S, Z, J, L) with unique colors.
- **Game Mechanics**:
  - Move pieces left/right (`a`/`d`).
  - Rotate clockwise (`w`) or counterclockwise (`s`).
  - Hard drop (`spacebar`).
  - Hold piece (`c`) with swap functionality.
  - Pause/resume (`p`/`r`).
- **Difficulty Levels**: Easy, Medium, Hard with adjustable drop speeds.
- **Scoring**: Points awarded based on lines cleared (100, 300, 500, 800 per level for 1-4 lines).
- **Level Progression**: Increases every 10 lines cleared, speeding up the game.
- **Customizable Board**: Set width and height at startup.
- **Highscore**: Tracks the session's highest score.
- **Menus**: Interactive main menu, mode selection, and play-again options with arrow key navigation.

## 🛠Requirements
- **Operating System**: Windows (uses `windows.h` and `conio.h` for console manipulation).
- **Compiler**: Any C++ compiler supporting C++11 or later (e.g., MinGW, MSVC).
- **Libraries**: Standard C++ libraries (`<bits/stdc++.h>`) and Windows-specific headers.

## How to Compile and Run
1. **Clone or Download**: Obtain the source code (`tetris.cpp`).
2. **Compile**:
   - Using MinGW: `g++ tetris.cpp -o tetris.exe`
   - Using MSVC: Open in Visual Studio and build the project.
3. **Run**: Execute the compiled binary (`tetris.exe`) in a Windows Command Prompt or double-click the executable.
   - *Note*: Ensure the console window is maximized for the best experience.

## 🎮Gameplay Instructions
1. **Start**: Launch the game, enter board width (min 10 recommended) and height (min 20 recommended).
2. **Main Menu**:
   - Use arrow keys (`up`/`down`) to navigate, `Enter` to select.
   - Options: Start, Highscore, Exit.
3. **Game Setup**:
   - Enter your name.
   - Choose difficulty: Easy (300ms drop), Medium (200ms), Hard (100ms).
4. **Controls**:
   - `a`: Move left
   - `d`: Move right
   - `w`: Rotate clockwise
   - `s`: Rotate counterclockwise
   - `space`: Hard drop
   - `c`: Hold piece
   - `p`: Pause
   - `r`: Resume
5. **Objective**: Clear lines by filling rows with blocks. Game ends when blocks stack to the top.

## 🖥️Code Structure
- **Tetromino Class**: Manages piece shapes, rotation, and positioning.
- **TetrisGame Class**: Core game logic, including grid management, rendering, and input processing.
- **Menu Functions**: Handle user interface and selections.
- **Main Loop**: Orchestrates game flow with custom board size, difficulty, and replay options.
- **Constants**: Shape definitions, colors, and speeds defined globally.

## ❌Limitations
- Windows-only due to reliance on `windows.h` and `conio.h`.
- Console-based rendering may flicker or behave inconsistently on some systems.
- No persistent highscore saving (resets each session).

## How To Run

1. Compile the program using a C++ compiler (MinGW/GCC recommended):

```bash
  g++ tetris.cpp -o tetris
```
2. Run
```bash
  tetris.exe
```

## 📜License
This project is unlicensed and free to use or modify for personal or educational purposes. Credit to the original author is appreciated.
