# Yahtzee scorecard

A single-file scorecard for playing Yahtzee with **real dice**. Roll the dice at the table, then tap the box you want to score. The app does the math, tracks whose turn it is, and keeps the running totals.

No build step, no dependencies, no accounts. Open `index.html` and play.

## Features

- 1 to 8 players, editable names, each with their own color
- Turn tracking: the active player is highlighted and play moves on after each score
- Clear highlighting of which boxes are still open, especially for whoever's turn it is
- Upper section helper: pick how many dice showed the number and it works out the points
- One-tap fixed scores (Full house 25, Small straight 30, Large straight 40, Yahtzee 50) or scratch the box
- On-screen number pad for 3 of a kind, 4 of a kind and Chance (0 to 30)
- Automatic 35-point upper bonus at 63+, with a progress meter
- Yahtzee bonus counter (+100 each)
- Undo for any input, as many steps back as you need (button in the header, or Ctrl/Cmd+Z)
- Winner banner with tie handling
- Vertical layout for phones, horizontal scoreboard layout for wide screens (switches at 1040px)
- Light and dark theme (follows system, with a manual toggle)
- Game state is saved in the browser (`localStorage`), so a refresh won't lose your game

## Run it

Just open `index.html` in any modern browser (double-click it, or drag it into a browser window). Nothing to install.

The page loads the "Fredoka" font from Google Fonts. If you're offline it falls back to the system font; everything else works with no internet connection.

## Host it online (optional)

Push this folder to a GitHub repo, then in the repo go to **Settings → Pages**, choose "Deploy from a branch", pick `main` and `/ (root)`, and save. It'll be live at `https://<your-username>.github.io/<repo-name>/`.

Any static host works too (Netlify, Vercel, Cloudflare Pages, itch.io, a plain S3 bucket) — it's one HTML file.

## Files

- `index.html` — the whole app: HTML, CSS and JavaScript in one file
- `LICENSE` — MIT

## License

MIT. See [LICENSE](LICENSE).
