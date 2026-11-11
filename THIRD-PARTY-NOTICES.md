# Third-party notices

OpeningsTrainer (formerly Mtrainer) is a personal tool whose built web app is published
for the owner's own devices. Because it bundles **chessops** (GPL-3.0-or-later) and sounds
under AGPL-3.0-or-later, the project is marked `GPL-3.0-or-later` in `package.json`; the
GPL/AGPL obligations (source availability, license text, notices) apply to the whole
distributed application.

Runtime dependencies bundled into `dist/` (versions pinned in `package-lock.json`):

| Package | Version | License | Source |
|---|---|---|---|
| chessops | 0.15.1 | GPL-3.0-or-later | https://github.com/niklasf/chessops |
| @badrap/result | 0.3.1 | MIT | https://github.com/badrap/result |
| react | 19.3.0 | MIT | https://github.com/facebook/react |
| react-dom | 19.3.0 | MIT | https://github.com/facebook/react |
| scheduler | 0.28.0 | MIT | https://github.com/facebook/react |
| react-chessboard | 5.12.1 | MIT | https://github.com/Clariity/react-chessboard |
| @dnd-kit/core | 6.3.1 | MIT | https://github.com/clauderic/dnd-kit |
| @dnd-kit/modifiers | 9.0.0 | MIT | https://github.com/clauderic/dnd-kit |
| @dnd-kit/utilities | 3.2.2 | MIT | https://github.com/clauderic/dnd-kit |
| @dnd-kit/accessibility | 3.1.1 | MIT | https://github.com/clauderic/dnd-kit |
| dexie | 4.4.5 | Apache-2.0 | https://github.com/dexie/Dexie.js |
| fflate | 0.8.3 | MIT | https://github.com/101arrowz/fflate |
| tslib | 2.8.1 | 0BSD | https://github.com/microsoft/tslib |
| @supabase/supabase-js (and its @supabase/* packages) | 2.119.0 | MIT | https://github.com/supabase/supabase-js |

Sounds in `public/sounds/` (served as files, not modified):

| File | Origin | License |
|---|---|---|
| Move.mp3, Capture.mp3 | Lichess "standard" sound set (lila, `public/sound/standard`), as used by Listudy | AGPL-3.0-or-later — https://github.com/lichess-org/lila |
| success.mp3, error.mp3 | Listudy (`assets/static/sounds/other`) | AGPL-3.0 — https://github.com/ArneVogel/listudy |

The full license texts ship inside each package in `node_modules/<package>/LICENSE*`.
Chess piece graphics are the default set bundled in react-chessboard (MIT). No fonts,
images or scripts are loaded from the network; the UI uses fonts installed on the system.
The only network connection is the optional account sync to the owner's Supabase project.

Development-only tools (not bundled): TypeScript 6.0.3 (Apache-2.0), Vite 8.3.3 (MIT),
@vitejs/plugin-react 6.1.1 (MIT), Vitest 5.0.3 (MIT), Playwright 1.63.0 (Apache-2.0),
fake-indexeddb 6.2.5 (Apache-2.0).

Course files imported by the owner remain the owner's private material. They are never
copied into this repository, its fixtures or its documentation.
