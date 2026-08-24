# SessionSnap update check endpoint

This repo exists only to publish `version.json`, a small public file the SessionSnap app checks
on startup to see if a newer version is available. It's a separate public repo because the actual
SessionSnap source lives in a private repo, and GitHub Pages (or any public raw-file access) isn't
available for private repos on a free plan.

**No product code lives here.** To release a new version of SessionSnap: build it, publish it
wherever it's distributed, then update `version` (and optionally `releaseUrl`/`notes`) in
`version.json` and push. The app picks up the change automatically on its next startup check.

Raw file used by the app:
`https://raw.githubusercontent.com/SessionSnap/updates/main/version.json`
