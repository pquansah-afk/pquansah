# Prince Quansah — Personal Site

A single-page career site: about, experience, farm photos, education, awards, and a downloadable CV.

## Files

```
index.html              the whole page
assets/style.css         all styling
assets/images/           farm + portrait photos
assets/files/Prince_Quansah_CV.pdf   your CV, linked from the "Download CV" buttons
```

## 1. Open it in VS Code

1. Unzip this folder somewhere on your computer, e.g. `prince-site/`.
2. In VS Code: **File → Open Folder…** and choose `prince-site`.
3. Install the **Live Server** extension (search it in the Extensions panel) so you can preview changes.
4. Right-click `index.html` → **Open with Live Server** to see the site in your browser as you edit.

Things you'll likely want to personalize:
- Your LinkedIn URL — add it next to the email/phone in the **Contact** section of `index.html` (search for `contact-links`).
- Any wording in the hero, about, or timeline sections — just edit the text between the HTML tags.
- Swap or add photos in `assets/images/` and reference them the same way the existing ones are referenced.
- Colors and fonts live at the top of `assets/style.css` under `:root`, if you want to adjust the palette later.

## 2. Put it on GitHub Pages

**Option A — brand-new site (e.g. `princequansah.github.io`):**

1. On GitHub, create a new repository named exactly `<your-username>.github.io`.
2. In VS Code's terminal, from inside the `prince-site` folder:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. Your site will be live at `https://<your-username>.github.io` within a minute or two — no extra settings needed for a `username.github.io` repo.

**Option B — a project page instead (e.g. `github.com/<you>/portfolio`):**

1. Create a repo with any name, e.g. `portfolio`.
2. Push the same way as above but to that repo's URL.
3. On GitHub: **Settings → Pages → Source**, choose the `main` branch and `/ (root)` folder, then **Save**.
4. Your site will be live at `https://<your-username>.github.io/portfolio/`.

## 3. Updating later

Any time you edit files in VS Code:
```bash
git add .
git commit -m "Update site"
git push
```
GitHub Pages rebuilds automatically after each push.
