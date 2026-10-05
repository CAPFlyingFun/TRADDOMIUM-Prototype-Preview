# TRADDOMIUM Chapter One hybrid preview

Separate GitHub Pages build of source **94bdd5b068c69e1ad2b4411ab8a64c00e6fc23d5**.
Source: https://github.com/CAPFlyingFun/TRADDOMIUM-Micro-Battle/tree/94bdd5b068c69e1ad2b4411ab8a64c00e6fc23d5/prototype

Production main, Main-Backup, the island/legacy build and PR #9 remain unchanged.
Original models, artwork and recorded audio load from the pinned source commit.
No asset binaries are duplicated here.

New Game opens the canonical date/island/cloud descent and then the 3D laboratory.
Scripted dialogue and character staging alternate with exploration intervals.
Select Jack or Sarah (once she arrives). Desktop: WASD/arrows, C to switch.
Portrait: tap clear floor to move. Touch landscape also has a held-direction pad.
Objective buttons walk the selected character to the target before interacting.
Characters return to their scripted positions before dialogue resumes.
Auto shot restores cinematic direction after manual camera orbit/pan/zoom.
Pause preserves exploration positions and clears held movement.
Laboratory progress remains session-only; Continue is disabled.

Validation: 29 focused tests, typecheck, production build, rig decoding and all
206 startup asset hashes (16,289,594 bytes). Actual WebGL browser checks cover the
opening, keyboard movement, pause/resume, terminal objectives, intercom, Sarah's
arrival/selection, and portrait/landscape controls. Physical iPhone review remains
necessary. Navigation handles static furniture; it is not crowd simulation.

Rebuild in source prototype/: PREVIEW_SOURCE_SHA=94bdd5b068c69e1ad2b4411ab8a64c00e6fc23d5 node scripts/build-preview.mjs
Copy dist-preview here. Asset inventory/provenance and implementation notes are
in prototype/docs/ in the source repository.
