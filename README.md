# Culture Shock

A single-file roguelike for studying clinical bacteriology lab tests. Open `index.html` in any browser, desktop or phone. It needs no build step and no external libraries.

- Each room is a patient with an unknown organism. Run lab-test cards (each costs lab budget) to reveal pixel-art results, then identify the organism. A wrong ID costs HP.
- After each case, pick 1 of 3 rewards: a new test, an upgrade, or healing.
- Bosses are look-alike pairs that need the one test that separates them.
- Permadeath. Floors unlock in order: Enterics → Non-enterics → Mixed Ward.
- The Codex unlocks an organism's full results once you've identified it.
- Progress is saved in `localStorage`.

## Editing the data

All organism results are in the `ORGANISMS` table at the top of `index.html`. A comment above it explains the value codes. The boss pairs and their study notes are in `BOSSES` just below it. A test that separates a boss pair is worked out automatically from the table.
