# Penform

**Turn your handwriting into a real font.**

Penform lets you write out characters by hand, scan them, and export a working `.ttf` font you can use in Word, Pages, and anywhere else on your Mac.

---

## Requirements

- macOS 12 or later (Apple Silicon or Intel)
- No Python or other software required — Penform is a standalone app

---

## Installation

1. Open `Penform-Installer.dmg`
2. Drag **Penform** into your Applications folder
3. On first launch, right-click the app and choose **Open** (required once to bypass Gatekeeper on unsigned builds)

---

## Getting Started

When you first open Penform, you'll be asked to choose a workflow:

- **Draw in App** — draw characters directly on screen using your mouse or trackpad
- **Print & Scan** — print a template, write on paper, scan or photograph it, and import

Both workflows end at the same place: a glyph library you can export as a `.ttf` font. If this popup doesn't appear, click the settings icon, click reset preferences, then quit and reopen the app.

---

## Print & Scan Workflow

This is the recommended workflow for the most natural-looking results.

### Step 1 — Choose Characters
- Click **+ Add Characters to Library** and select a character pack (e.g. Basic Latin)
- Your library will show empty slots for each character

### Step 2 — Generate & Print Template
- Click **Next: Print Template**
- Save the PDF and print it
- Each page has a grid of boxes — write each character inside its box
- Use the guidelines to keep your letters at a consistent size:
  - **Top blue line** — cap height (for tall letters like A, B, H)
  - **Blue dashed line** — x-height (for lowercase like a, c, e)
  - **Solid baseline** — where letters sit
  - **Orange dashed line** — descender depth (for g, p, q, y)

### Step 3 — Scan & Upload
- Scan or photograph your completed template pages
  - Good lighting, flat surface, no shadows
  - PDF or image files both work
- Click **Choose Photo or PDF** and select your file
- Penform reads the QR code on each page to automatically map characters

### Step 4 — Export Font
- Go to the **Export** tab
- Click **Export TTF**
- Save to Downloads (default)
- Double-click the `.ttf` file and click **Install Font**

---

## Draw in App Workflow

1. Select a character from your library
2. Draw it on the canvas using your mouse or trackpad
3. Use the guidelines to match proportions
4. Repeat for each character
5. Export TTF when done

---

## Tips for Best Results

- **Write naturally** — don't try to be too precise, natural variation is what makes the font look handwritten
- **Consistent size** — try to keep letters at a similar size relative to the guidelines on each page
- **Dark ink on white paper** — ballpoint or felt tip works best, avoid pencil or light ink
- **Scan at high resolution** — 300 DPI or higher if scanning; photos work too as long as the page is flat and well-lit
- **Multiple passes** — you can re-import a template to overwrite specific characters

---

## Exporting & Installing Your Font

After exporting a `.ttf` file:

1. Double-click the file in Finder
2. Click **Install Font** in Font Book
3. Open Word, Pages, or any app and search for your font name in the font picker

To update your font with new characters, export a new `.ttf` with the same font name and reinstall — Font Book will replace the old version.

---

## Troubleshooting

**"Penform is damaged and can't be opened"**

This is a macOS security warning for apps downloaded from outside the App Store. Penform is safe — here's how to fix it:

1. Click **Cancel** (do not move to Trash)
2. Open **Terminal** (search for it in Spotlight with Cmd+Space)
3. Run this command:
```
xattr -cr /Applications/Penform.app
```
4. Try launching Penform again normally

This only needs to be done once after installing.

---

**App takes a long time to open on first launch**

Normal — the app unpacks itself on first run. Give it 10–15 seconds.

---

## Known Limitations (Beta)

- Unsigned app — requires right-click → Open on first launch
- First launch may take 10–15 seconds while the app unpacks
- Very small punctuation marks (` ' " .`) may require good lighting to scan correctly
- Uppercase letters may have slightly different sizing than lowercase in some handwriting styles

---

## Feedback

This is an early beta. If something doesn't work as expected, please share:
- What workflow you were using
- Which step it failed at
- A screenshot if possible

Thanks for testing!
