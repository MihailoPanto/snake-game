# Snake Game (Zmijica)

A classic Snake game built with HTML5, JavaScript, jQuery, and Bootstrap. No installation or build process required — runs directly in any modern browser.

## Demo / How to Run

Open `zmijica-uputstvo.html` directly in any modern browser. No installation or server needed.

## Pages

| File | Purpose |
|------|---------|
| `zmijica-uputstvo.html` | Start page — instructions and settings (entry point) |
| `zmijica-igra.html` | Game board |
| `zmijica-rezultati.html` | High scores and last result |

**Navigation flow:**

```
Instructions/Settings → Play → Results → Instructions/Settings
```

## Gameplay

- Control the snake using **arrow keys**
- Eat food to grow longer and earn points
- Avoid colliding with walls or your own body
- Win by filling the entire grid with your snake

### Food

| Type | Appearance | Points | Behavior |
|------|-----------|--------|----------|
| Normal food | Green `F` | +1 | Always present; respawns after being eaten |
| Super food | Gold `S` | +10 | Spawns every 10 seconds; disappears after 3–9 seconds |

## Settings

Configured on the start page and saved in `localStorage`.

### Board Size

| Option | Grid |
|--------|------|
| Small | 10×10 |
| Medium (default) | 15×15 |
| Large | 20×20 |

### Difficulty

| Level | Snake speed |
|-------|------------|
| Easy | 300 ms/move |
| Normal (default) | 200 ms/move |
| Hard | 100 ms/move |

## Scoring

- Current score shown in real time during the game
- Top 5 high scores saved per browser (via `localStorage`)
- Enter your name on the results page to save your score

## Tech Stack

- **HTML5 / CSS3 / JavaScript** — core game logic and layout
- **jQuery 3.6.4** — DOM manipulation and event handling
- **Bootstrap 3.3.7** — UI components and styling
- **localStorage** — settings and score persistence (no backend needed)

All dependencies are bundled locally in the `zmijica-dodatno/` directory.

## Project Structure

```
SnakeGame/
├── zmijica-uputstvo.html     # Start/settings page
├── zmijica-uputstvo.js       # Settings page logic
├── zmijica-igra.html         # Game page
├── zmijica-igra.js           # Game engine
├── zmijica-rezultati.html    # Results/leaderboard page
├── zmijica-rezultati.js      # Results page logic
├── zmijica.css               # Shared styles
└── zmijica-dodatno/          # Bundled dependencies
    ├── jquery-3.6.4.js
    ├── bootstrap.min.css
    └── bootstrap.min.js
```
