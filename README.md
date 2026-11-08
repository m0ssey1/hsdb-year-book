# Leave Your Mark: 2026 Yearbook (Digital Mock-up)

Interactive digital yearbook mock-up for [School Name], in the school colours (red, black and yellow) with the Wil en Werk badge.

## Files
- `index.html`: the entire yearbook (self-contained; badge and styles are built in)
- `.nojekyll`: tells GitHub Pages to serve the file as-is
- `README.md`: this file

## Before you publish
Open `index.html` in a text editor and search for `DOC_URL`. Replace the link with your documentary link:

```js
const DOC_URL="https://example.com/our-documentary";
```

The "Watch the documentary" buttons and both QR codes use this one line.

Also search for `[School Name]`, `[Town]`, `[Principal Name]` and `[Documentary Title]` and replace them with your real details.

## Publish on GitHub Pages
1. Create a new repository (for example `yearbook-2026`).
2. Upload `index.html`, `.nojekyll` and `README.md` to the repository root.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select branch `main` and folder `/ (root)`, then Save.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Notes
- The QR codes are generated in the browser with the qrcodejs library from cdnjs, so the page needs an internet connection.
- Fonts load from Google Fonts. Without internet, readable fallback fonts are used.
- Time Capsule notes are saved in each learner's own browser only.
- Portraits, signatures and statistics are placeholders.
