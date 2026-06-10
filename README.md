# Personal site — GitHub Pages

A single-page personal/academic site. Static HTML, **no build step**.

## 1. Fill in the placeholders (search `index.html`)
- `[username]` → your GitHub username
- `[your-email]` → your McGill email (appears twice: contact nav + footer)
- `assets/Clinton_Gao_CV.pdf` → **export your CV (`.docx`) to PDF** (Word → Save As → PDF) and drop it in `assets/`
- `assets/comp550_implicit_negation.pdf` → **already included** ✅
- (optional) uncomment the LinkedIn link, and the "Notes & explorations" section at the bottom

## 2. Deploy to GitHub Pages
1. On GitHub, create a **new public repo named `<your-username>.github.io`** (exact name → this becomes a *user site*).
2. From this folder, commit and push (your own first commit — keeps the public history 100% yours):
   ```bash
   git init
   git add -A
   git commit -m "Initial personal site"
   git branch -M main
   git remote add origin git@github.com:<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. Wait ~1 minute → live at **https://&lt;your-username&gt;.github.io**

   *User sites enable Pages automatically. If you instead use a differently-named repo (a "project site"), go to Settings → Pages → Source: `main` branch.*

## 3. Preview locally
Double-click `index.html`, or:
```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Notes
- Content mirrors your CV (honest scoping). If you update the CV, update the matching lines here.
- The `in progress` tags are intentional — keep them honest.
- Once you confirm the Finance project's DSR/PBO status, tighten the "robust backtesting methodology" line to match.
