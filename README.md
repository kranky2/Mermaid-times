# Mermaid Times

A sea-themed times tables game (2× to 12×) for phones, with a weekly goal.

- **Practice Lagoon** – no clock, number pad, pick tables, optional "both ways" (4 × 3 and 3 × 4) and tricky fish mixed in. Wrong answers get a tip, like "3 × 8 = 24, and one more group of 8 makes 32".
- **Race the Tide** – one table (all 12 facts shuffled) or a mix of tables (6 questions per table: 4 random + 2 tricky fish). No lives; 100 points per right answer plus up to 50 for speed. Beat your best score.
- **Tricky Fish** – any fact she gets wrong or takes over 8 seconds on. It is set free after 3 right in a row, each under 8 seconds, over at least 2 different days. Each direction (4 × 3 vs 3 × 4) is tracked separately.
- **Weekly goal** – 4 days out of Monday–Sunday. A day counts after one finished race or 20 practice questions. The treasure is agreed with a grown-up and typed in on the Grown-ups page.
- **Grown-ups** (hold the button for 2 seconds) – 11 × 12 grid of every fact, direction trouble, slowest tables, recent weeks.

The "4 groups of 3" line fades out for each fact as she gets it right in a row.

Progress is saved in the phone's browser. Single `index.html`, no build step.

## Shell Sums (`sums.html`)

Untimed column addition and subtraction, laid out like a worksheet.

- Toggles: Add / Minus / Mix · Tens / Hundreds · carrying or borrowing: No / Some / Every sum.
- A page of 10 sums. She fills in the answer one column at a time from the ones, can tap dotted circles to write a carried 1, and can tap a top digit to borrow from it.
- Wrong answers show which column to look at; after one try, "Show me how" explains each column.
- The home screen shows how often each kind of sum is right first time.
- **Three-number sums** (separate section): three numbers stacked in one column sum, like 22 + 33 + 3, 55 − 17 − 18 or 45 + 20 − 18. Add / Minus / Mix, tens or hundreds. Carry marks and borrowing go up to 2, since three numbers can need it. "Show me how" works down each column.

## Offline

Both games work offline after they have been opened once with internet (a service worker keeps a copy on the phone). Pages still update automatically whenever the phone is online.

## Pearl Tingxie (`chinese.html`)

Chinese spelling (听写) for the P1 1B lists, lessons 15 to 19. Every word is practised both ways:

- **Write the word:** she sees the Hanyu Pinyin and hears the word, then writes the characters with her finger, stroke by stroke (or on paper, then checks against animated strokes). Characters in brackets on the school list are shown in grey and not tested.
- **Write the pinyin:** she sees the characters and types the pinyin on a letter keyboard, then taps a letter and a tone to place the tone mark. It checks letters, tone and where the mark sits.
- **Strokes (笔画):** she draws the named stroke inside an example character (横折弯 in 朵, 横折斜钩 in 风, 斜钩 in 我, 卧钩 in 心).
- **Mock 听写:** one lesson exactly as the school tests it, scored out of the total.
- **Tricky words:** anything missed comes back until it is right 2 times in a row on 2 different days.

Pinyin for section 二 words is not on the school list, so standard Hanyu Pinyin is used; common alternatives (like xué sheng / xué shēng) are accepted.

Character drawing uses [Hanzi Writer](https://hanziwriter.org) (MIT, see `LICENSE-hanzi-writer.txt`) with stroke data from hanzi-writer-data (Arphic Public License, see `ARPHICPL.TXT`). Both are bundled, so it works offline too.
