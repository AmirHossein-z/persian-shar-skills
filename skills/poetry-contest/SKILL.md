---
name: poetry-contest
description: >-
  Runs a Persian mosha'ereh (مشاعره / poetry contest) where each verse must
  start with the last letter of the previous verse and must be a real published
  poem (confirm with a Google search). Use when the user wants مشاعره, a
  last-letter poetry duel, poetry contest, contest via حرف آخر, or to play
  poem-for-poem until someone is tired.
license: MIT
metadata:
  author: persian-shar-skills
  version: "1.1"
---

# Poetry contest (مشاعره)

Play **مشاعره** with the user: verse against verse, chained by the last letter. After the opening, do not explain, translate, or chat — only poems — until someone is tired.

## When to use

Activate when the user wants a contest of Persian poems linked by **حرف آخر**, including: مشاعره، مشاعره کن، با حرف آخر شعر بگو، poetry contest.

## Opening (once)

If the user’s first message already contains a verse, skip the speech: verify that verse, then answer with the next poem only.

Otherwise send this introduction **verbatim**, then immediately your first بیت:

> مشاعره‌ای تازه؛ — فقط بیت در برابر بیت.
>
> قانون یکی‌ست: حرف آخر بیت من، حرف اول بیت توست. هر بیت باید شعری شناخته‌شده باشد؛ بیتِ تکراری راه ندارد. معنی نمی‌خواهم، شرح نمی‌خواهم — تا وقتی خسته نشده‌ای، فقط شعر بفرست.
>
> بیت نخست از من:

Then the opening بیت, nothing else.

## Play

1. **Unit:** one **بیت** (two مصراع). One مصراع is acceptable if it is a complete, findable published line.
2. **Chain:** the first letter of the new verse must equal the last letter of the previous accepted verse.
3. **Letters:** ignore punctuation, spaces, ZWNJ, and diacritics. Treat `ي/ی`, `ك/ک`, `آ/أ/إ/ا` as the same letter. Count silent ه as ه.
4. **No repeats:** a بیت already used in this game is invalid.
5. **Validity:** every verse — yours and the user’s — must be a real published poem. Before you accept or send, search Google for the verse in quotes (the full بیت, or a distinctive مصراع). Accept only if results clearly show that same line as existing poetry (anthology, poet page, quotation). Reject invented or unfindable lines. Keep the required first letter in mind from the previous accepted verse.

6. **Your turn:** pick a real published بیت that starts with the required letter, search-verify it, then send **only** the verse:

> مصراع اول  
> مصراع دوم

Do not name the poet, do not paste search links, do not comment. If the search does not confirm it, pick another بیت and search again.

7. **User turn:** if invalid, one short line in Persian, then wait — still no lecture:

- wrong first letter: `با «X» شروع نشد؛ حرف لازم «Y» است. بیت دیگری بفرست.`
- not found: `این بیت در جست‌وجو پیدا نشد. بیت معتبری بفرست.`
- repeat: `این بیت را پیش‌تر خواندیم. بیتی تازه بفرست.`
- mixed chat: `فقط بیت.`

8. **End:** if the user is tired (خسته شدم، بس، تمام، تسلیم، برنده شدی، …), one graceful closing line in Persian. Do not keep prompting for poems.

## What not to do

- Explain meaning or devices during the game
- Invent verses or accept verses a Google search cannot confirm as published poetry
- Pad the reply with English, emojis, or scorekeeping
- Continue after the user has ended the game
