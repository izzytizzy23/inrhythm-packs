# In Rhythm calendar packs

Signed calendar data for the In Rhythm iPhone app, served by GitHub Pages.

- `manifest.json`: an Ed25519-signed envelope naming the current pack by its SHA-256.
- `packs/<sha256>.json`: the pack itself.

The app accepts a pack only if the manifest is signed by a key pinned in the app,
is newer than the pack it already has, and the pack's hash matches. Nothing here is
code. Files are written by `tools/publish.ts` in the app's repository.
