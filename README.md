# Disc Transition Comms Coach

A scripted training chatbot for C&G Assignment 3. It coaches employees, managers and stakeholders on how to communicate an unpopular company decision to the public. It is built from our report on Sony Interactive Entertainment's announcement ending disc production for new PlayStation games from January 2028.

Student project. Not affiliated with or endorsed by Sony Interactive Entertainment.

## How to open it

- **Online:** open the GitHub Pages link for this repository.
- **Offline:** download `index.html` and double-click it. It opens in any web browser. No installation is needed. An internet connection is only used to load the fonts.

## How it works

- The bot has a fixed bank of 23 questions with prepared answers. It does not use AI.
- When you type a question, it scores each prepared answer by the keywords and phrases it finds. Strong phrases count 3 points, supporting words 1 point, and words from the question title 0.5 points. If the best score reaches 2.5, it gives that answer.
- If the match is weak, it suggests the closest questions. If nothing matches, it says so and offers starting points.
- Each answer shows which keywords it matched, so the logic is visible.
- Answers are grouped under the five communication failures identified in the report: wrong audience, too late, defensive, lost control of the voice, and abstract and incomplete. There is also a planning checklist.

## Editing the answers

All questions, keywords and answers are in the `BANK` list near the top of the `<script>` section in `index.html`.
