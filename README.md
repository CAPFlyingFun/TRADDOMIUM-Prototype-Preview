# TRADDOMIUM Chapter One test preview

Separate GitHub Pages browser test build of candidate **1807e261e7345ef7aa33637c9e76bc1da35deee2**.
Source: https://github.com/CAPFlyingFun/TRADDOMIUM-Micro-Battle/tree/1807e261e7345ef7aa33637c9e76bc1da35deee2/prototype

The existing game repository's main, Main-Backup, Pages site, legacy build and
unmerged PR are not changed. This is not a promotion of the candidate.

The browser bundle is served here. Original models, artwork and recorded audio
are fetched from the pinned public candidate commit, not a moving branch.
Asset/model provenance remains in the source repository's prototype/docs/.

Use New Game for Chapter One. Laboratory progress is session-only. Continue is
disabled. This is camera/object control, not free player walking.

Source checks: typecheck/build, 14 focused tests, exact-model rig checks and 201
asset hashes pass. The Replit browser runner has WebGL disabled; actual rendered
gameplay, audible playback and iPhone Safari need device review before promotion.

Rebuild recipe: use the source's Vite config at the pinned commit, base './',
define import.meta.env.BASE_URL as the assetBase from preview.json, and set
publicDir false. This leaves runtime logic unchanged while isolating hosting.
