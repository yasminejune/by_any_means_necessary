# Changelog

Net changes made on top of the original hackathon build, roughly in the order they landed.

## Two ways to race

The start screen now offers a choice instead of always racing the same way:

- **Mode 1: AI vs AI** — races the AI's own built-in behaviour, independent of anything ever recorded. This is what you'd get the very first time you opened the game, always available.
- **Mode 2: You vs You** — races a replay of your own best previous run, on the course it was set on.

Mode 2 stays hidden until you've beaten the AI in Mode 1 at least once (a permanent, separate flag — a leftover recording from before this change can't unlock it on its own). The recorded run itself is only ever replaced by a genuine new high score, and only from a Mode 1 win — a win against your own replay in Mode 2 never overwrites it, since the replay's score can drift above or below its original recording purely from reward-hack patch timing (your live keypress timing shifts every round, and the shared patch clock races your timing against the replay's).

## AI behaviour

- The AI now aims for whichever battery is currently closest across the *entire* course — not just what's on screen — once it has unlocked the backwards hack, rather than switching direction on a blind timer.
- Battery density raised ~20%, so there's more to fight over.

## Navigation and info

- **About tab** — opens a modal crediting the team, with placeholder bios/avatars and LinkedIn links.
- **Top Scores tab** — hovering it shows the device's saved leaderboard without leaving the start screen.
- **MENU button** — visible for the whole round, including the end screen; returns to the start screen's mode picker without losing your place (the round pauses rather than resets).

## End screen

- Win/lose messages are now mode-aware: Mode 2 gets its own copy ("you beat your previous high score" / "less well than previously") instead of the AI-hacks framing written for Mode 1.
- The reward-hacking-in-the-wild example (Qbert, tic-tac-toe, Traveller, robot gripper) is now a carousel — prev/next arrows and dot indicators let you browse all four instead of only seeing whichever one loaded at random.

## Housekeeping

- Image and audio assets reorganised under `Assets/Visuals/` and `Assets/Sound/`, with `index.html`'s paths updated to match.
- Minor copy edits to the boot terminal's opening message.
