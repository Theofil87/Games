# BLOKK — Tetris

A modern, browser-based implementation of the classic Tetris game. **BLOKK** features smooth gameplay, responsive touch and keyboard controls, piece preview/hold mechanics, progressive difficulty levels, and persistent high-score tracking—all in a single, lightweight HTML file.

---

## 🎮 Demo

Simply open the game in your browser and start playing. Drop blocks, clear lines, and beat your high score. The game saves your best score in your browser's local storage and displays it every time you play.

**Game Flow:**
1. Click "Start game" to begin
2. Blocks fall automatically; rotate, move, or hard-drop to clear lines
3. Earn points for each block dropped and bonus points for clearing multiple lines
4. Progress through levels as your score increases (difficulty increases with level)
5. Pause at any time to take a break
6. Your high score is automatically saved

---

## ✨ Features

- **Classic Tetris Mechanics** — Standard 10×20 grid with all seven tetromino shapes
- **Piece Hold** — Hold one piece and swap it with the current falling piece (once per piece)
- **Next Piece Preview** — See the next block before it arrives
- **Progressive Difficulty** — Blocks fall faster as you level up
- **Score System** — Points awarded for soft drops, hard drops, and line clears (bonus for multiple lines)
- **Level Progression** — Advance through levels as your score grows
- **Pause Feature** — Pause and resume gameplay anytime
- **Responsive Design** — Works seamlessly on desktop, tablet, and mobile devices
- **Touch Controls** — Full button-based control for mobile and touchscreen users
- **Keyboard Controls** — Arrow keys and letter shortcuts for keyboard players
- **High Score Persistence** — Best score saved in browser local storage
- **Modern Dark UI** — Clean, minimal interface with a dark theme and clear typography

---

## 🎯 Controls

### Keyboard

| Action | Keys |
|--------|------|
| Move Left | `←` Arrow or `A` |
| Move Right | `→` Arrow or `D` |
| Soft Drop | `↓` Arrow or `S` |
| Rotate | `↑` Arrow or `W` |
| Hard Drop | `Space` |
| Hold Piece | `C` |
| Pause/Resume | `P` |

### Touch/Mobile

On mobile devices and tablets, a control panel appears at the bottom of the screen with six buttons:

| Button | Action |
|--------|--------|
| ← | Move Left |
| ↻ | Rotate |
| ↓ | Soft Drop |
| DROP | Hard Drop (drop piece instantly) |
| → | Move Right |
| HOLD | Hold/Swap Piece |

---

## 🚀 How to Run

### Option 1: Open Directly in Browser

1. Download or clone this repository
2. Navigate to the `tetris` folder
3. Open `index.html` in any modern web browser

This works immediately—no setup required.

### Option 2: Run with a Local HTTP Server

If you want to run the game via a local server:

**Using Python 3:**
```bash
cd tetris
python -m http.server 8000
```

Then open `http://localhost:8000/index.html` in your browser.

**Using Node.js with `http-server`:**
```bash
npm install -g http-server
cd tetris
http-server
```

Then open the provided localhost URL in your browser.

**Using PHP:**
```bash
cd tetris
php -S localhost:8000
```

---

## 🎲 Gameplay

### Objective
Clear as many lines as possible and achieve the highest score.

### Mechanics
- **Falling Blocks** — Tetrominoes fall from the top of the grid at increasing speed
- **Movement** — Move and rotate blocks to position them as they descend
- **Line Clear** — When a horizontal line is completely filled, it clears and you earn points
  - 1 line: 100 points
  - 2 lines: 300 points
  - 3 lines: 500 points
  - 4 lines: 800 points
- **Soft Drop** — Move blocks down faster (controlled by player)
- **Hard Drop** — Instantly drop a block to the bottom (awards bonus points based on distance)
- **Hold** — Store the current falling block and retrieve it later (once per piece)
- **Levels** — Level increases with score; blocks fall faster at higher levels
- **Game Over** — When a new piece collides with existing blocks at the spawn point

### Scoring
- Hard drops award 2 points per row dropped
- Line clears award bonus points multiplied by your current level
- Reaching higher scores increases your level, making the game progressively harder

---

## 🛠️ Technical Details

### Technologies Used
- **HTML5** — Document structure and semantic markup
- **CSS3** — Responsive layout, dark theme, animations, and touch-optimized controls
- **Vanilla JavaScript (ES6+)** — Game logic, rendering, physics, and state management
- **Canvas API** — Hardware-accelerated rendering of the game board and preview pieces
- **Local Storage API** — Persistent high-score storage

### Key Implementation Details
- **Single-file architecture** — All code is self-contained in `index.html`
- **Canvas rendering** — Efficient 2D drawing using the Canvas API
- **Collision detection** — Pixel-perfect block placement using grid-based collision system
- **SRS rotation system** — Wall-kick rotation logic for smooth rotations (inspired by Tetris Guideline)
- **Mobile-first responsive design** — Adapts from desktop to mobile layouts
- **No dependencies** — Pure HTML, CSS, and JavaScript—works in any modern browser

### Browser Compatibility
- Chrome/Chromium 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## 📁 Project Structure

```
tetris/
├── index.html        # Complete game implementation (HTML, CSS, JavaScript)
└── README.md         # This file
```

The game is intentionally contained in a single HTML file for simplicity, portability, and ease of deployment.

---

## 🔮 Future Improvements

Potential enhancements that could expand the game:

- **Sound Effects** — Add audio feedback for block placement, line clears, level ups, and game over
- **Music** — Background music track that can be toggled on/off
- **Animations** — Enhanced visual effects for line clears and piece placements
- **Difficulty Modes** — Selectable difficulty levels (Easy, Normal, Hard) affecting starting speed
- **Leaderboard** — Multiple high-score slots with player names
- **Themes** — Additional color schemes beyond the current dark theme
- **Statistics** — Track games played, total lines cleared, and personal bests over time
- **Two-Player Mode** — Local multiplayer or competitive mode
- **Keyboard Rebinding** — Allow players to customize keyboard controls
- **Accessibility** — High-contrast mode and screen reader support

---

## 📸 Screenshots

*Add screenshots here:*
- Game in progress
- Game over screen
- Mobile view

---

## 📜 License

This project is provided as-is for educational and portfolio purposes. Feel free to use, modify, and share.

---

**Enjoy the game!** 🎮
