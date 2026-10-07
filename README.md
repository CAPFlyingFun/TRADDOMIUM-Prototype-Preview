# TRADDOMIUM Chapter One hybrid preview

Separate GitHub Pages build of source **3c84509d128d78501204ea0e59b77067b5af3d37**.
Source: https://github.com/CAPFlyingFun/TRADDOMIUM-Micro-Battle/tree/3c84509d128d78501204ea0e59b77067b5af3d37/prototype

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

2026-10-07: toon Jack and Sarah (Pixar-style models). Sarah's bump is re-weighted so it
keeps its shape seated, she sits in a pregnancy-aware posture, and she no longer types or
sleeps unscripted (PR #10). Sarah's fingers are rigged.

Validation: 42 focused tests, typecheck, production build, rig decoding and all
216 startup asset hashes (17,029,641 bytes). Actual WebGL browser checks cover the
opening, keyboard movement, pause/resume, terminal objectives, intercom, Sarah's
arrival/selection, and portrait/landscape controls. Physical iPhone review remains
necessary. Navigation handles static furniture; it is not crowd simulation.

Rebuild in source prototype/: PREVIEW_SOURCE_SHA=3c84509d128d78501204ea0e59b77067b5af3d37 node scripts/build-preview.mjs
Copy dist-preview here. Asset inventory/provenance and implementation notes are
in prototype/docs/ in the source repository.
