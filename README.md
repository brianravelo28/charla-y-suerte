# Charla y Suerte

A two-player "War"-style conversation-practice game for language tutoring, built as a single self-contained HTML file.

A randomizer (cards, dice, wheel, or coin) decides a winner and loser each round; the loser answers a prompt built from a topic, word bank, and — at higher levels — a sub-topic, all drawn from pools spanning CEFR levels A1–C2. Word bank chips and topics support hover/press-and-hold Spanish glosses.

## Usage

Open `index.html` directly in a browser — no build step, no dependencies, no backend.

## Structure

Everything (markup, styles, and game logic) lives in `index.html`. The game state machine covers:

- **Setup flow**: game mechanic → level → topic scope, each choice staying visible as the next one appears
- **Word banks**: verbs (Level A), adjectives/adverbs/prepositional phrases (Levels B/C), plus a wrong-answer toggle for added difficulty
- **Topics & sub-topics**: category-coded (personal, tense-focused, structural) with large rotating pools to avoid repetition
- **Companion guide**: a slide-out reference panel with example sentences and quick word lists per level
