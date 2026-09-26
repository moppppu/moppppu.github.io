# Research Homepage — GitHub Pages starter

A minimal academic homepage inspired by simple research profile pages such as `theory-and-me.github.io`.
It is intentionally plain HTML/CSS so that updating publications does not require a framework or build tool.

## 1. Customize before publishing

Edit `index.html` and replace:

- `Shoichiro Takeda` if needed
- the short bio / research interests
- `#` links for Google Scholar, GitHub, and CV
- `YOUR_EMAIL@example.com`
- placeholder Work Experience and Education
- the publication list

### Profile photo

Put your photo at:

```text
assets/profile.jpg
```

Then change this line in `index.html`:

```html
<img class="portrait" src="assets/profile-placeholder.svg" alt="Profile placeholder">
```

to:

```html
<img class="portrait" src="assets/profile.jpg" alt="Shoichiro Takeda">
```

A portrait crop around 600 x 720 px works well.

## 2. Publish with GitHub Pages — easiest browser-only method

1. Sign in to GitHub.
2. Create a new repository named exactly:

   ```text
   YOUR_GITHUB_USERNAME.github.io
   ```

3. Make the repository public if you are using GitHub Free.
4. Upload the contents of this folder **to the root of the repository**. `index.html` must be at the repository root.
5. Open the repository's **Settings**.
6. Open **Pages** in the left sidebar.
7. Under **Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
8. Click **Save**.
9. Open:

   ```text
   https://YOUR_GITHUB_USERNAME.github.io/
   ```

Future edits are published when you commit changes to `main`.

## 3. Publish from your computer with Git

Create the GitHub repository first, then run from inside this folder:

```bash
git init
git add .
git commit -m "Create research homepage"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME.github.io.git
git push -u origin main
```

Then enable GitHub Pages in **Settings -> Pages** as described above.

For later updates:

```bash
git add .
git commit -m "Update publications"
git push
```

## 4. Add a new publication

Copy one `<li>...</li>` block inside `<ol class="publications">` in `index.html`, then edit the authors, title, link, venue, and year.

Example:

```html
<li>
  <span class="authors"><strong>Shoichiro Takeda</strong>, Coauthor.</span>
  <a class="paper-title" href="https://example.com/paper">Paper title.</a>
  <span class="venue">Conference, 2026.</span>
</li>
```

## 5. Optional: use a custom domain

You do **not** need a custom domain. `YOUR_GITHUB_USERNAME.github.io` works perfectly well for an academic homepage.

If you later buy a domain, configure it under **Settings -> Pages -> Custom domain** and follow GitHub's DNS instructions. Enable HTTPS once the domain is verified.

## File structure

```text
research-homepage/
├── index.html
├── style.css
├── .nojekyll
├── README.md
└── assets/
    └── profile-placeholder.svg
```
