# Kids Memory Match

Kids Memory Match is a four-level SVG card-matching game.

## How it plays

The player flips two cards at a time and tries to find identical SVG images.

**flip first card → flip second card → match or mismatch → update lives → complete all pairs → advance level**

Progression:

- Level 1: 2 pairs / 4 cards
- Level 2: 3 pairs / 6 cards
- Level 3: 4 pairs / 8 cards
- Level 4: 5 pairs / 10 cards

Each level starts with three lives. A mismatch removes one life. Completing a level restores three lives for the next level. Victory is reached after the available SVG image set has been used through the progression.

## Implementation

The playable frontend is a React application in `frontend/`.

Key implementation details:

- React state manages level, cards, flipped cards, matched cards, lives, timer and fullscreen state.
- SVG card artwork is loaded from `frontend/public/cards/`.
- card pairs are shuffled for each level;
- Framer Motion handles interface/card animation;
- `react-confetti` is used for completion feedback;
- fullscreen mode is supported;
- the backend folder contains a separate FastAPI/MongoDB status-check scaffold and is not required by the visible game loop.

## Event activation

This game was developed as one module in a multi-game interactive children’s edutainment activation in the UAE.

Event production: [Peach Society](https://peach-society.com/) — Dubai-based event and experiential production company.

## Related implementation

`kids-match`, `kids-svg`, and `kids-svg-game` contain closely related Memory Match development states. They are separate repository records of the same game family.
