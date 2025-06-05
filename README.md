# One Piece TCG Deck Registration

This project is a tool for One Piece TCG players who want a simple, no-login solution to register their decks, convert formats, and print them in a clean and readable format.

It was heavily inspired by [seitrox's sim2cardmarket converter](https://seitrox.github.io/optcg-sim2cardmarket-converter/), a fantastic open-source project that laid the foundation for this one. You should definitely check it out—and if you find either project helpful, consider donating over there to support the work!

## Try It Out

* [https://hugoprudente.github.io/optcg-to-deck-registration-sheet/](https://hugoprudente.github.io/optcg-to-deck-registration-sheet/)

---

## What's in this repo?

This repository includes two main components:

- 🔎 A scraper that pulls card data from official One Piece TCG sources
- 🌐 A lightweight frontend to register, display, and print decks from `.txt` format (sim/export format)

---

## Features

✅ **Uppercase and lowercase card search**
Search for cards easily without worrying about capitalization.

✅ **Dual card list support**
Includes both **en** (English) and **asian-en** card lists—merged and filtered for duplicates.

✅ **Card stats link**
Click on a card to view its stats and rulings on **[gumgum.gg](https://gumgum.gg)**.

✅ **Printable output**
Clean, formatted deck display with a **"Print / Save as PDF"** button—works if you have compatible print drivers installed.

---

## How to Use the Scraper

The scraper fetches cards from [https://en.onepiece-cardgame.com/cardlist](https://en.onepiece-cardgame.com/cardlist) and [https://asia-en.onepiece-cardgame.com/cardlist](https://asia-en.onepiece-cardgame.com/cardlist), processes the data, and exports:

- A well-formatted `.txt` file with full card info
- A detailed `.csv` version
- A condensed `.csv` version with only card IDs and names (no alts)

The scraper caches HTML files of each set (e.g., OP01, OP02) to avoid redownloading unnecessarily (1-hour cache timeout, configurable).

### Prerequisites

- Python 3  
- pip

### Setup

```bash
# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

```

# Run the scraper

python src/scraper.py

## Contributions

Let me know if you’d like this version saved as a file or need a version that includes screenshots, badges, or deployment instructions.
