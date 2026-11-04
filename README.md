# training_note

Personal training log. Static site on GitHub Pages: https://kaitokurokochi.github.io/training_note/

- **Form**: record a day's exercises (weight / reps per set) and notes
- **History**: entries by date, filterable by exercise
- **Chart**: per-exercise trend (max weight / volume / estimated 1RM)

## Data

- `data/log.json` — all entries
- `data/exercises.json` — exercise names shown in the form dropdown

Saving from the form commits these files through the GitHub API.

## Setup (once per device)

Create a fine-grained personal access token limited to this repository with **Contents: Read and write**, then paste it into the Form tab. It is kept only in the browser's `localStorage`; never commit it.
