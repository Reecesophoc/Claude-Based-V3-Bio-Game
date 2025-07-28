# Claude-Based-V3-Bio-Game

This repository contains `V3.html`, a browser-based game for learning the basics of DNA replication. It runs entirely in the browser, so no build step is required.

## Opening the game

1. Clone or download the repository.
2. Locate `V3.html` and open it with any modern browser (Chrome, Firefox, Edge, etc.).
3. The page will load the game interface directly from the file system—no server is required.

## Gameplay basics

- When the game loads, you will be asked to enter a name and begin training.
- Select complementary DNA bases from the pool (A pairs with T, G pairs with C) and click the matching position on the new strand.
- Progress through increasing levels to complete the replication sequence. Every fifth level is a boss encounter.
- Watch your health and XP bars; completing sequences quickly and accurately awards experience points.
- Use the **Check Replication** button when all bases are placed to finish a sequence.

## Node environment check

A small Node script `check.js` is provided to verify that Node.js is installed correctly:

```bash
node check.js
```

Running the command should print:

```
Node environment is working!
```

This check is optional but helps confirm your environment can execute Node.js scripts if you plan to extend the project.

## Recommended environment

- Any up‑to‑date web browser to play the game.
- Node.js (v18 or later recommended) if you want to run the Node check or develop additional tooling.

