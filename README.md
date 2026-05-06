# NEXRIS — Cyberpunk Tetris

> A sleek, single-file cyberpunk block-puzzle game built with pure HTML, CSS, and the Web Audio API.

🎮 **Play it live:** [https://teohweibin.github.io/nexris-tetris/](https://teohweibin.github.io/nexris-tetris/)

---

## Features

### 🎮 Core Gameplay
- **Classic Tetris mechanics** — 10×20 board with all 7 standard tetrominoes (I, O, T, S, Z, J, L)
- **7-bag randomizer** — pieces are drawn from a shuffled bag, ensuring fair distribution
- **SRS-lite rotation** — wall-kick support (up to ±2 columns) for smooth piece rotation
- **Ghost piece** — a translucent preview shows exactly where the current piece will land
- **Hold piece** — swap the active piece into a hold slot and retrieve it later

### 📈 Progression
- **10 speed levels** — the game accelerates every 10 lines cleared, from 800 ms/drop at level 1 down to 100 ms/drop at level 10
- **Level progress bar** — a visual indicator shows how close you are to the next level
- **High score persistence** — your personal best is saved in `localStorage` and displayed across sessions

### 🎨 Visual Themes
Switch between **5 colour themes** at any time using the theme buttons at the bottom of the screen:

| # | Theme      | Accent Colours         |
|---|------------|------------------------|
| 1 | Cyberpunk  | Cyan / Hot Pink        |
| 2 | Retro      | Orange / Yellow        |
| 3 | Ocean      | Light Blue / Deep Blue |
| 4 | Synthwave  | Magenta / Purple       |
| 5 | Matrix     | Bright Green / Dark Green |

Your chosen theme is saved to `localStorage` and restored on your next visit.

### ✨ Visual Effects
- **Animated background grid** — a scrolling cyber-grid lines the background
- **Neon glow rendering** — every piece is drawn with a matching colour glow using Canvas shadows
- **Particle burst** — each cleared row explodes into glowing particles
- **Screen flash** — the board flashes briefly on a line clear

### 🔊 Sound Effects (Web Audio API)
All sounds are synthesised in real-time — no audio files required:

| Event         | Sound                                  |
|---------------|----------------------------------------|
| Piece locked  | Short square-wave thump                |
| Line cleared  | Ascending 4-note sine chime            |
| Game over     | Descending 4-note sawtooth dirge       |

### ⏸ Pause & Resume
- Press **ESC** to pause the game — an overlay appears showing *PAUSED*
- Press **ESC** again or click the **RESUME** button to continue

---

## Controls

| Key           | Action                      |
|---------------|-----------------------------|
| `←` / `→`    | Move piece left / right     |
| `↑`           | Rotate piece clockwise      |
| `↓`           | Soft drop (one row)         |
| `Space`       | Hard drop (instant lock)    |
| `Shift`       | Hold / swap piece           |
| `Esc`         | Pause / Resume              |

---

## Scoring

Points are awarded per line-clear and scaled by the current level:

| Lines Cleared | Points (× Level) |
|---------------|-----------------|
| 1             | 100             |
| 2             | 300             |
| 3             | 500             |
| 4 (Tetris)    | 800             |

---

## How to Play

NEXRIS is a **zero-dependency, single-file web app**.

1. Open `index.html` in any modern browser.
2. Click **START GAME** (or press the button on the overlay).
3. Clear lines, climb levels, and beat your high score!

No installation, build step, or internet connection required (fonts load from Google Fonts if online).

---

## Tech Stack

| Technology        | Usage                                     |
|-------------------|-------------------------------------------|
| HTML5 Canvas      | Board rendering, pieces, particles, previews |
| CSS Variables     | Theme switching and neon glow palette     |
| Web Audio API     | Procedural sound effects                  |
| `localStorage`    | High score & theme persistence            |
| Google Fonts      | *Orbitron* (headings) & *Rajdhani* (UI)  |

---

## File Structure

```
nexris-tetris/
└── index.html   # Complete game — HTML, CSS, and JavaScript in one file
```

---

## License

This project is open source. Feel free to fork, remix, and build on it.
