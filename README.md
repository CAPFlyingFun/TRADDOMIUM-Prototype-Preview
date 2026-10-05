# TRADDOMIUM Chapter One test preview

Separate GitHub Pages browser test build of candidate **c5e7c51eb2255043a7ed24d400a1152973b92637**.
Source: https://github.com/CAPFlyingFun/TRADDOMIUM-Micro-Battle/tree/c5e7c51eb2255043a7ed24d400a1152973b92637/prototype

The existing game repository's main, Main-Backup, Pages site, legacy build and
unmerged PR are not changed. This is not a promotion of the candidate.

The browser bundle is served here. Original models, artwork and recorded audio
are fetched from the pinned public candidate commit, not a moving branch.
Asset/model provenance remains in the source repository's prototype/docs/.

Use New Game for Chapter One. Its byte loader downloads 206
assets (16289594 bytes; 16.3MB),
then shows the canonical Story date/island/cloud descent before entering the lab.
Narration and character staging are automated; camera and console actions are
manual. Playback reuses downloaded assets in this tab without a second transfer.
Laboratory progress is session-only. Continue is disabled. This is camera/object
control, not free player walking.

Source checks: typecheck/build, 21 focused tests, original-model rig tests and 206
asset hashes pass. Browser checks cover the byte loader, automatic date/island,
portrait/landscape, pause/resume and lab handoff/title recovery. The runner has
WebGL disabled; the updated hosted build still needs iPhone review before promotion.

Rebuild recipe: use the source's Vite config at the pinned commit, base './',
define import.meta.env.BASE_URL as the assetBase from preview.json, and set
publicDir false. This leaves runtime logic unchanged while isolating hosting.
