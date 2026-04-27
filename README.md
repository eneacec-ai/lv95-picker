# lv95-picker

A Trimble Connect extension that picks points in the 3D viewer and exports them as LV95/LN02+ coordinates in CSV format.

Hosted on GitHub Pages: `https://eneacec-ai.github.io/lv95-picker/`

---

## Branches

| Branch | Purpose |
|--------|---------|
| `BugFix` | Active development |
| `main` | Production — GitHub Pages serves from here |

---

## Workflow

### 1. Make changes

Work on the `BugFix` branch:

```bash
git checkout BugFix
# edit index.html
git add index.html
git commit -m "describe your change"
git push origin BugFix
```

### 2. Deploy and test in Trimble Connect

Merge to `main` to publish via GitHub Pages:

```bash
git checkout main
git merge BugFix
git push origin main
```

GitHub Pages updates within ~1 minute. The extension in TC automatically loads the new version on next open.

### 3. Register the extension in TC (first time only)

1. Open your TC project
2. Go to **Settings → Extensions → Custom Extensions**
3. Paste the manifest URL: `https://eneacec-ai.github.io/lv95-picker/manifest.json`
4. Click **Add**

---

## Manifest

`manifest (1).json` points to the GitHub Pages URL and does not need to be changed.
