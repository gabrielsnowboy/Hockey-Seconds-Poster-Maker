# Hockey Seconds Poster Maker

Make "hockey seconds" fundraiser posters in your browser:

- Add names and tick who has paid ✓
- Choose a table format:
  - **15 rows**: 30 spots of 2 seconds (01/02 … 59/00) in two columns
  - **18 rows**: 36 numbered spots (1–36) in two columns
  - **30 rows**: 60 spots of 1 second (:00 – :59) in two columns
  - Each format keeps its own list of names
- Pick any NHL matchup. All 32 teams' 2025–26 logos are built in.
- Set the date, time, prizes and price per spot
- Choose a theme: Gothic romance, Burgundy & gold, Blush & roses, Ice rink, or Black & gold
- Export as **PNG, JPG, WEBP or PDF** in poster (3:4), post (4:5), square or Story (9:16) sizes
- Share straight to Facebook, Instagram and other apps from your phone

Everything you enter stays on your own device. Nothing is uploaded anywhere.

---

## Put it on GitHub Pages (about 5 minutes)

1. Sign in at **github.com** and click **+ → New repository**.
   - Name it something like `hockey-seconds-poster`.
   - Set it to **Public** (free GitHub Pages needs a public repository).
   - Click **Create repository**.
2. On the new repository page, click **uploading an existing file**.
3. Unzip `hockey-seconds-poster-site.zip` on your computer, open the folder, and drag **everything inside it** into the GitHub page:
   `index.html`, `sw.js`, `manifest.webmanifest`, `og-image.jpg`, `README.md`, `.nojekyll` and the `icons` folder.
   (On a Mac, press ⌘ + Shift + . in Finder to see the hidden `.nojekyll` file. The app works without it if you skip it.)
4. Click **Commit changes**.
5. Go to **Settings → Pages**. Under **Build and deployment**, set
   **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**, then click **Save**.
6. Wait a minute or two, then refresh the page. GitHub shows your link, for example:
   `https://YOUR-USERNAME.github.io/hockey-seconds-poster/`

### Optional: nicer link previews on Facebook
Open `index.html` on GitHub (pencil icon ✏️ to edit), find this line:

```html
<meta property="og:image" content="og-image.jpg">
```

and change it to your full address, for example:

```html
<meta property="og:image" content="https://YOUR-USERNAME.github.io/hockey-seconds-poster/og-image.jpg">
```

---

## Using it like an app

- **Computer (Chrome / Edge):** click **Install app** in the top-right corner, or the install icon in the address bar.
- **Android:** open the link in Chrome → **⋮ → Install app / Add to Home screen**.
- **iPhone / iPad:** open the link in Safari → **Share → Add to Home Screen**.

After the first visit, the app also works **offline**.

## Keeping your work

- The app saves your board and logos in the browser automatically.
- Click **Save project** to keep a backup file (`.json`). It includes your names, settings and any logos you added yourself. Use **Open project** to load it on another computer or browser.

## Updating the app later

1. Upload the new `index.html` to the repository (it replaces the old one).
2. Open `sw.js` and change `const VERSION = 'v1.3.0';` to a new number, for example `'v1.3.1'`.
3. Commit. People who already have the app see **"A new version of the app is ready — Reload"**.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app |
| `sw.js` | Offline support and update notices |
| `manifest.webmanifest` | Lets the app be installed |
| `icons/` | App icons |
| `og-image.jpg` | Picture shown when the link is shared |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
