# Kids Memory Match

Kids Memory Match is a four-level SVG card-matching game developed within the same multi-game interactive children’s edutainment activation in the UAE as the other `kids-*` game repositories.

## Game structure

The player flips two cards at a time and attempts to match identical SVG images.

**flip first card → flip second card → match or mismatch → update matched cards/lives → complete all pairs → advance level**

The current frontend implements:

- Level 1: 2 pairs / 4 cards
- Level 2: 3 pairs / 6 cards
- Level 3: 4 pairs / 8 cards
- Level 4: 5 pairs / 10 cards

Each level starts with three lives. A mismatched pair removes one life. Completing a level restores three lives for the next level. Victory occurs after the available SVG image set has been used through the progression.

## Repository structure

- `frontend/` — React memory-matching game and SVG card assets
- `backend/` — FastAPI/MongoDB status-check scaffold
- `tests/` and `test_reports/` — historical test material
- `test_result.md` — historical test summary

The visible game logic in `frontend/src/App.js` does not depend on the backend status-check routes.

## Related repository lineage

The current `frontend/src/App.js` is byte-identical to the corresponding game file in `Joenasriani/kids-svg`, establishing a direct shared implementation state at the audited revisions.

Both repositories are preserved independently. This relationship does not authorize merging, deleting, renaming, archiving or replacing either repository.

## Deployment status

The repository Homepage field currently points to `https://kids-match.vercel.app`, which returned 404 during the audit. No working public deployment is therefore claimed here.

## Preservation boundary

The frontend, backend, SVG assets, level progression, lives logic, matching behavior, timer behavior, animations, tests and historical development files are preserved. This documentation pass does not alter gameplay or runtime behavior.
