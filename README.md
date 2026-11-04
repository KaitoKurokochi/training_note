# training_note

Personal training log. Static site on GitHub Pages: https://kaitokurokochi.github.io/training_note/

- **Form**: record a day's exercises (weight / reps per set) and notes
- **History**: entries by date, filterable by exercise
- **Chart**: per-exercise trend (max weight / volume / estimated 1RM)

## Data

Records live in the private `KaitoKurokochi/vault` repo, not here:

- `health/training_note/log.json` — all entries
- `health/training_note/exercises.json` — exercise names for the form dropdown

Both are created on first save. The site reads and writes them through the GitHub Contents API, so this repo only holds the page code.

## Setup (once per device)

Create a fine-grained personal access token limited to `vault` with **Contents: Read and write**, then enter it on the first screen. It is kept only in the browser's `localStorage`; never commit it.
