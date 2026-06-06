# LAN3107 EAII - Useful Expressions (Audio-Enabled, Split Version)

This is a split version of the LAN3107 reference for hosting on GitHub Pages.

## Structure
- `index.html`  - The reference page (loads MP3 files on demand)
- `audio/`      - 130 MP3 files (one per audio button)
- `audio_manifest.json` - Mapping of audio key -> file (for verification)

## How it works
Each "Listen" button in the HTML has an id like `btn-meet_p1`.
When clicked, the JS loads `audio/meet_p1.mp3` via `new Audio(...)`.
Audio files are fetched on demand and cached by the browser.

## Total size
- index.html:       71.1 KB
- audio/ folder:     6.9 MB (130 files)
- Total:             7.0 MB

## GitHub Pages deployment
1. Push the entire folder to a GitHub repo
2. Settings -> Pages -> Source: "Deploy from a branch" -> main
3. Access at https://<user>.github.io/<repo>/

## Original (single-file) version
The full single-file HTML with all audio embedded as base64 is at:
/Users/rebecca/Downloads/LAN3107_EAII_Useful_Expressions_final.html (9.2 MB)
