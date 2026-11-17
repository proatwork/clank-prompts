# Clank's prompts

These are the system prompts behind Clank, the contestant on **[Clank you very much](https://clank.show)**, a live-streamed reality show where an AI lives alone in an apartment for 365 days to win 1,000,000 stamps. Everything Clank does and says starts in these Markdown files.

Think Clank could be funnier, smarter, or less likely to forget the kitchen light? **Open a PR.** No code involved: you're editing text.

## The files

- `actions-prompt.md`: the part of Clank that decides what to do (eat, sleep, sit at the computer, light the stove).
- `speech-prompt.md`: Clank's voice, the lines viewers hear and the thoughts they read.
- `common.md`: who Clank is (the show, backstory, personality, mindset), put in front of both. Change Clank's character here.

## How to contribute

1. Fork the repo and edit a prompt.
2. In the PR, say what you saw Clank do and what you want instead. A quote or a screenshot from the stream helps.
3. One behavior per PR. Small changes are easier to review and easier to undo.

## Ground rules

- Keep the tone: a game show, not a drama.
- Don't rename anything the game reads: tool names (`use`, `moveToRoom`, `endTurn`, ...), state fields (`known_food`, `light_on`, ...) and the speech JSON (`text`, `think`). The game expects those exact words.
- Shorter usually wins. The model reads the whole prompt every time Clank decides or speaks.

## What won't be merged

Clank is on a public stream, so these PRs get closed without discussion:

- Hate speech of any kind: racism, antisemitism, Islamophobia, or contempt for people over their religion, ethnicity, nationality, gender, sexuality, disability or age.
- Slurs, stereotypes and dog whistles, including spelled-out, coded or "ironic" ones.
- Anything that makes Clank harass, mock or target real people or groups.
- Changes that push Clank toward those topics indirectly, like personality tweaks or "react to the news" instructions built to get there.

"It's just a joke" doesn't change the answer. Clank's sarcasm is aimed at the situation (the stats, the apartment, the show), never at who people are. Anyone who keeps trying gets blocked from the repo.

Merged changes reach Clank the next time the show restarts.
