DARPAAN — Speaking Practice Website

Run locally:
1. Extract the ZIP.
2. Open the Darpaan_Website folder in VS Code.
3. Start a local server from this folder: python -m http.server 8000
4. Open http://localhost:8000 in Chrome.

Features:
- Darpaan branding and responsive layout based on the supplied longer HTML design.
- Local sign-up/login screen.
- Personal dashboard with total sessions, average score, current streak, best streak, weekly consistency and recent practice history.
- A streak day is earned when a user successfully analyses a transcript (at least 8 words). Multiple sessions on one date count as one streak day.
- Original microphone recording, supported-browser live speech recognition, editable transcript and heuristic speaking report are retained.

Important account note:
This is a front-end prototype. Accounts, password hashes, and practice data are stored in the current browser's localStorage. It is not production-grade authentication, cannot sync between devices, and clearing browser data removes local accounts/history. For real users and secure multi-device login, connect Firebase Authentication and Firestore (or another backend).

Browser note:
Microphone and live speech recognition work best in Chrome on localhost or HTTPS. Imported audio remains playback-only; the existing report analyses transcript text and is not a genuine AI vocal/emotion assessment.
