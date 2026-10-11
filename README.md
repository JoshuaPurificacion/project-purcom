# PurCom study room

A mobile-first Purposive Communication reviewer based on the supplied class notes.

## Open

Double-click `Open reviewer.cmd`, or open `index.html` in a browser. No installation or build is required. The app uses
classic scripts so it also works directly from the file system.

For a local server, run `python -m http.server 8765 --bind 0.0.0.0` in this folder,
then visit `http://localhost:8765`. To open on a phone on the same Wi-Fi network,
use the computer's local IP address with port 8765. The computer must keep running
and its firewall must permit that connection.

## Practice

- All 12 topics support identification and enumeration.
- Flashcards follow topic order, with shuffled cards inside each topic.
- Quizzes use typed answers, partial enumeration credit, and practice or exam modes.
- Accept equivalent wording manually if the built-in checker rejects it.
- Progress is stored in the current browser. It does not sync between devices.
- Short explanations added for list-only notes are visibly marked as study aids.
- Google Fonts is optional; system fonts take over without internet access.

## Files

`data.js` contains the notes and answer alternatives. `app.js` contains study flows
and answer checking. `styles.css` contains responsive styling.

## Verification

Run `node tests.cjs` for content coverage, answer-checking, and study-flow checks.
