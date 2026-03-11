# The Count

A single-file blackjack simulator built for mobile. No accounts, no ads, no casino nonsense — just a clean table, real rules, and AI players that actually behave like humans.
Play by going to aenlow.github.io/The-Count, it is also mobile-friendly, so play it on your phone too!
---

## What it is

The Count is a browser-based blackjack game that simulates a real Vegas table experience. You pick your seat, bots fill the rest, and play unfolds left to right just like sitting down at a casino. The goal isn't to gamble — it's to practice, learn table dynamics, and understand how the people around you affect your hand.

---

## Features

**Table**
- 1, 6, or 8 deck shoe with crypto-quality shuffle
- H17 rules (dealer hits soft 17) · 3:2 blackjack · double after split
- Up to 4 AI bots at a 5-seat table
- Staggered left-to-right card deal animation
- Hole card flip animation on dealer reveal
- Live shoe burn bar (green → amber → red as shoe depletes)

**AI Bots**
- Three difficulty levels — Novice, Regular, Shark
- Novice plays scared: stands too early, never splits or doubles
- Regular follows basic strategy ~78% of the time with realistic human mistakes
- Shark plays perfect basic strategy every hand
- Bots have their own chip stack, go broke, cash out, and get replaced by a new player after a random number of hands — just like a real table

**Betting**
- Chip selection ($5 / $25 / $100 / $500)
- Nudge buttons (±$25)
- REPEAT / DOUBLE / MAX shortcuts
- Last bet auto-loads between hands

**Seat Picker**
- All seats start empty — you pick your spot first
- Bots fill the remaining seats around you
- Returns to seat picker between sessions, stays at table between hands

---

## Rules

| Rule | Setting |
|------|---------|
| Dealer soft 17 | Hit (H17) |
| Blackjack pays | 3:2 |
| Double down | Any first 2 cards |
| Double after split | Yes |
| Split aces | One card each, no re-split |
| Insurance | Offered when dealer shows Ace |
| Shoe penetration | Reshuffles at 25% remaining |

---

## How to run

No build step. No dependencies. One file.

```bash
git clone https://github.com/yourname/the-count.git
cd the-count
open blackjack.html
```

Or just open `blackjack.html` directly in any modern browser. Works offline.

For mobile, add to home screen via Safari (iOS) or Chrome (Android) for a fullscreen app-like experience.

---

## Keyboard shortcuts

| Key | Action |
|-----|--------|
| `H` | Hit |
| `S` | Stand |
| `D` | Double |
| `P` | Split |

---

## Project structure

```
the-count/
└── blackjack.html    # entire game — HTML, CSS, and JS in one file
└── README.md
```

---

## Roadmap

- [ ] Dealer running total during draw phase
- [ ] Auto-advance timer between hands
- [ ] Bot balance bars
- [ ] Session summary on exit
- [ ] Basic card counting trainer mode (hi-lo running count overlay)

---

## License

MIT — do whatever you want with it.
