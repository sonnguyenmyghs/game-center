# 🎮 Game Center

A collection of 38 browser-based games — playable instantly with no install, no dependencies, and no backend. Every game is a single self-contained HTML file with inline CSS and JavaScript.

## 🕹️ Play

Open `index.html` in any modern browser, or serve the folder with any static file server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

---

## 🎯 Games

### Classic Arcade
| Game | Description |
|------|-------------|
| [2048](2048/) | Swipe to merge tiles and reach 2048 |
| [Flappy Bird](flappy-bird/) | Tap to fly through pipes |
| [Snake](snake/) | Classic snake — eat, grow, survive |
| [Dino Runner](dino-runner/) | Endless runner, jump over obstacles |
| [Breakout](breakout/) | Bounce the ball to break all bricks |
| [Tetris](tetris/) | Rotate and stack falling blocks |
| [Stack Tower](stack-tower/) | Time your taps to stack blocks perfectly |
| [Knife Hit](knife-hit/) | Throw knives at a spinning log |
| [Hole.io](hole-io/) | Grow your black hole by swallowing objects |

### Puzzle
| Game | Description |
|------|-------------|
| [Sudoku](sudoku/) | Classic 9×9 number puzzle |
| [Wordle](wordle/) | Guess the 5-letter word in 6 tries |
| [Memory Card](memory-card/) | Flip and match pairs |
| [2048](2048/) | Merge numbers to reach the target |
| [Color Sort](color-sort/) | Sort colored balls into matching tubes |
| [Block Blast](block-blast/) | Place blocks to clear rows and columns |
| [Merge Numbers](merge-numbers/) | Combine numbers on a grid |
| [Suika Game](suika-game/) | Drop and merge fruit |

### Board & Strategy
| Game | Description |
|------|-------------|
| [Tic-Tac-Toe](tic-tac-toe/) | Classic X vs O — play vs AI |
| [Solitaire](solitaire/) | Klondike card solitaire |

### Casual
| Game | Description |
|------|-------------|
| [Candy Crush](candy-crush/) | Match 3 candy puzzle |
| [Color Match](color-match/) | Tap the matching color fast |
| [Whack-a-Mole](whack-a-mole/) | Hit the moles before they hide |

### Reward / Minigames
| Game | Description |
|------|-------------|
| [Gift Box](gift-box/) | Pick a mystery box and reveal your prize |
| [Lucky Wheel](lucky-wheel/) | Spin the wheel for a random prize |
| [Scratch Card](scratch-card/) | Scratch to reveal 3 matching symbols |
| [Slot Machine](slot-machine/) | 3-reel slot machine with coin rain effects |

---

## 🎉 Seasonal Events

Themed variants of reward games for each major holiday.

### 🎑 Mid-Autumn Festival
| Game | Prizes |
|------|--------|
| [Mid-Autumn Gift Box](gift-box-trungthu/) | Mooncake sets, festival vouchers |
| [Mid-Autumn Lucky Wheel](lucky-wheel-trungthu/) | Mooncake vouchers, lantern gifts |
| [Mid-Autumn Scratch Card](scratch-card-trungthu/) | Moon festival jackpot, mooncake boxes |
| [Mid-Autumn Slot Machine](slot-machine-trungthu/) | Moon grand prize, festival star prizes |

### 🎄 Christmas
| Game | Prizes |
|------|--------|
| [Christmas Gift Box](gift-box-noel/) | Christmas jackpot, Santa gifts |
| [Christmas Lucky Wheel](lucky-wheel-noel/) | Holiday vouchers, mystery gifts |
| [Christmas Scratch Card](scratch-card-noel/) | Christmas tree, bells, snowflake prizes |
| [Christmas Slot Machine](slot-machine-noel/) | Christmas jackpot, Santa's grand gift |

### 🧧 Lunar New Year
| Game | Prizes |
|------|--------|
| [Lucky Red Envelope](gift-box-tet/) | Golden lucky money, New Year bonuses |
| [Lunar New Year Lucky Wheel](lucky-wheel-tet/) | Red envelopes, peach blossom gifts |
| [Lunar New Year Scratch Card](scratch-card-tet/) | Golden lucky money, fireworks prizes |
| [Lunar New Year Slot Machine](slot-machine-tet/) | Dragon jackpot, golden lucky money |

---

## 🏗️ Architecture

```
game-center/
├── index.html              # Hub — lists all games with category filter
├── <game-name>/
│   └── index.html          # Each game is fully self-contained
└── assets/                 # Shared static assets (if any)
```

**Each game file:**
- Single HTML file (~400–1000 lines)
- Inline `<style>` — no external CSS
- Inline `<script>` — no external JS
- Zero dependencies, zero build step
- Responsive — works on mobile and desktop
- Dark theme (`#0a0a1a` background)

---

## 🛠️ Tech

- **Vanilla HTML/CSS/JavaScript** — no frameworks
- **Canvas API** — used in Lucky Wheel, Scratch Card, some arcade games
- **requestAnimationFrame** — smooth 60fps animations
- **CSS animations** — seasonal particle effects (snowflakes, lanterns, fireworks)
- **Responsive design** — `clamp()`, `dvh`, flexbox/grid layouts

---

## 📦 Deployment

Since every file is static HTML, you can deploy anywhere:

```bash
# GitHub Pages — push to main branch, enable Pages in repo settings
git add .
git commit -m "Initial deploy"
git push origin main
```

Compatible with: GitHub Pages, Netlify, Vercel, any CDN or static host.

---

## 📝 License

MIT — free to use, modify, and distribute.
