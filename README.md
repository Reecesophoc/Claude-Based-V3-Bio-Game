# Claude-Based-V3-Bio-Game




This project is licensed under the [MIT License](LICENSE).

This repository contains `V3.html`, a browser-based game for learning the basics of DNA replication. It runs entirely in the browser, so no build step is required.

## Opening the game

1. Clone or download the repository.
2. Locate `V3.html` and open it with any modern browser (Chrome, Firefox, Edge, etc.).
3. The page will load the game interface directly from the file system—no server is required.

## Gameplay basics

- When the game loads, you will be asked to enter a name **and a nine‑digit student number** before beginning training.
- Select complementary DNA bases from the pool (A pairs with T, G pairs with C) and click the matching position on the new strand.
- Progress through increasing levels to complete the replication sequence. Every fifth level is a boss encounter.
- Mutation challenge levels occur every few rounds. Use Repair bases to fix damaged DNA before pairing.
- Watch your health and XP bars; completing sequences quickly and accurately awards experience points.
- Use the **Check Replication** button when all bases are placed to finish a sequence.
- Your progress is automatically saved in the browser. Returning players will be prompted to continue where they left off.

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

## Saving scores and server storage

Scores are stored locally in your browser under `dnaGameScores`. Each entry
contains the player's name, student number, XP, level reached, and the date.

To permanently record scores or receive an email notification you will need a
small server or third‑party service. A few possibilities are:

- **Node/Express server** – handle a `POST` request from the game and use
  libraries such as `nodemailer` or SendGrid to email results.
- **Google Sheets API** – create a script that appends rows to a spreadsheet for
  each submitted score.
- **Firebase or another hosted database** – store scores via a REST API and view
  them later through an admin page.

The game code only stores data locally; integrating one of these solutions would
allow centralized score tracking.

