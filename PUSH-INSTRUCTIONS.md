# Push to GitHub + enable Pages

Repo: https://github.com/sofortune81/SAI-translation

## 1. Push (run in this folder)

```bash
cd "C:\Users\Kelvin\Documents\DS Translation Test\gh-repo"

git init -b main
git add .
git commit -m "SAI Leisure Group 2025 annual report - Chinese translation, section 1"
git remote add origin https://github.com/sofortune81/SAI-translation.git
git push -u origin main
```

If GitHub rejects the push because the repo already has a commit (you ticked
"Add a README" when creating it), run this instead of the plain push:

```bash
git pull --rebase origin main
git push -u origin main
```

## 2. Enable Pages

Either in the browser:

**Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, folder `/ (root)` → Save**

Or with the `gh` CLI:

```bash
gh api -X POST repos/sofortune81/SAI-translation/pages \
  -f "source[branch]=main" -f "source[path]=/"
```

## 3. Your URL

Live 1–2 minutes after Pages finishes building:

**https://sofortune81.github.io/SAI-translation/**

The raw unstyled fragment stays available at `.../SAI-translation/chunk1.html`.

## Before you make it public

`index.html` is a machine-assisted translation of a listed company's annual report,
going out under your own GitHub account. If this is client work, consider keeping the
repo private — Pages on a private repo needs GitHub Pro.
