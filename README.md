# NEXRIS — Cyberpunk Tetris

> A neon-drenched, cyberpunk-themed Tetris clone built in a single HTML file — no dependencies, no build step required.

🎮 **[Play Now](https://teohweibin.github.io/nexris-tetris)**

---

## Features

- **Classic Tetris mechanics** — 10×20 board with all 7 standard tetrominoes (I, O, T, S, Z, J, L)
- **Ghost piece** — shows exactly where your piece will land
- **Hold piece** — swap the current piece to save for later
- **Next piece preview** — plan your moves in advance
- **10 levels** — speed ramps up every 10 lines cleared
- **Particle effects** — neon burst on every line clear
- **High score** — saved automatically via `localStorage`
- **Pause / Resume** — step away whenever you need
- **Cyberpunk aesthetic** — animated grid background, glowing neon blocks, Orbitron font

---

## Controls

| Key | Action |
|---|---|
| `← →` | Move left / right |
| `↑` | Rotate piece |
| `↓` | Soft drop |
| `Space` | Hard drop |
| `C` | Hold piece |
| `P` | Pause / Resume |

---

## Scoring

Points are multiplied by the current level.

| Lines Cleared | Points |
|---|---|
| 1 (Single) | 100 × level |
| 2 (Double) | 300 × level |
| 3 (Triple) | 500 × level |
| 4 (Tetris) | 800 × level |

---

## Levels

| Level | Drop Speed |
|---|---|
| 1 | 800 ms |
| 2 | 700 ms |
| 3 | 600 ms |
| 4 | 500 ms |
| 5 | 400 ms |
| 6 | 300 ms |
| 7 | 250 ms |
| 8 | 200 ms |
| 9 | 150 ms |
| 10 | 100 ms |

Level increases every 10 lines and caps at level 10.

---

## Running Locally

No build tools needed — just open the file in any modern browser.

```bash
git clone https://github.com/teohweibin/nexris-tetris.git
cd nexris-tetris
open index.html      # macOS
# or
start index.html     # Windows
# or
xdg-open index.html  # Linux
```

---

## Tech Stack

| | |
|---|---|
| Language | Vanilla HTML / CSS / JavaScript |
| Rendering | HTML5 Canvas 2D |
| Fonts | [Orbitron](https://fonts.google.com/specimen/Orbitron) · [Rajdhani](https://fonts.google.com/specimen/Rajdhani) via Google Fonts |
| Persistence | `localStorage` (high score) |
| Dependencies | None |

---

## License

This project is open source. Feel free to fork, remix, and build on it.
