# Musajala (المساجلة) — Arabic Poetry Duel Trainer

A Python tool for practicing **المساجلة الشعرية** (Arabic poetry dueling), where each contestant must answer with a verse that starts with the last letter of the opponent's verse.

🥈 **Using this tool, our team won 2nd place in the university poetry Musajala competition.**

## What it does

- Holds a collection of **~1,800 classical Arabic verses** (أبيات شعرية).
- Automatically groups every verse by its **opening letter** (أ، ب، ج، د ...), and prints how many verses are available for each letter.
- **Practice mode** — picks random letters and random verses so you can test whether you have them memorized, then prints a summary of the verses you still need to review, grouped by letter.

## How to use

Requires Python 3 (no external libraries).

```bash
python musajala.py
```

The script first prints all verses grouped by letter with counts, then asks:

1. `How Many bayet:` — how many rounds to practice.
2. `1 Or 0?` — choose the mode:
   - **`1`** — you type a letter (حرف) and get a random verse starting with it.
   - **`0`** — the program picks a random letter; answer `1` if you know a verse for it, or `0` to be shown one. Verses you didn't know are collected for review.

At the end, the verses from the session are listed by letter so you can focus your memorization.

## Adding verses

Add verses inside the `Abyat` string at the top of `musajala.py` — each verse as two lines (صدر و عجز) followed by a blank line.
