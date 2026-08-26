# groovepeek-docs

Public docs site for the **GroovePeek** and **PitchPeek** Chrome extensions.

Served at **https://damfernandes.github.io/groovepeek-docs/**

## Pages

- `index.html` — hub introducing both extensions
- `groovepeek.html` — GroovePeek (BPM detection)
- `pitchpeek.html` — PitchPeek (tuning reference)
- `privacy.html` — GroovePeek privacy policy
- `pitchpeek-privacy.html` — PitchPeek privacy policy
- `styles.css` — shared styles

`privacy.html` and the site root are registered on the live Chrome Web Store
listing, so **their paths must not change**.

## Screenshots

`store-assets/` holds captures of the shipping popups — real rendered UI, not
hand-built mockups, so the chrome cannot drift from what the extensions render.
The PitchPeek readings in them are scripted rather than measured from live audio;
keep each scene's values self-consistent (see the note in the harness).

- `screenshot-*.png`, `state-*.png` — GroovePeek
- `pp-state-*.png` — PitchPeek

The PitchPeek captures are generated from the harness in the extension repo
(`store-assets/pitchpeek/_harness/`), which serves the built `dist-tuning/`
bundle with the Chrome APIs stubbed so any popup state can be driven and shot.
