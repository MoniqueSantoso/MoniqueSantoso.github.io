# Academic Portfolio — Jekyll + GitHub Pages

A clean, minimal academic portfolio site. Hosted free on GitHub Pages.

---

## Quick Start

### 1. Create your GitHub repository

Create a new repo named **`yourusername.github.io`** (replace with your actual GitHub username).  
This makes your site live at `https://yourusername.github.io`.

### 2. Push this folder to GitHub

```bash
git init
git add .
git commit -m "Initial portfolio"
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

Go to your repo → **Settings → Pages → Source → Deploy from branch → main → / (root)**.

Your site will be live in ~1 minute at `https://yourusername.github.io`.

---

## Customizing Your Site

### Personal info
Edit **`_config.yml`** — update your name, title, institution, email, and social links.

### Bio / About
Edit **`index.html`** — find the `#about` section and replace the placeholder text with your own bio.

### Photo
Drop your headshot into `assets/images/headshot.jpg`, then uncomment the `<img>` tag  
in `index.html` and remove the placeholder `<div>`.

### Research papers
Edit **`_data/research.yml`** — add one entry per paper. Fields:
- `title` (required)
- `authors`, `venue`, `tags`, `award` (optional)
- `links` — list of `{label, url}` pairs (PDF, Code, Slides, etc.)

### Teaching
Edit **`_data/teaching.yml`** — add one entry per course. Fields:
- `name`, `code`, `role`, `term`, `description`

### CV
Drop your CV PDF into `assets/` as `cv.pdf`. The CV pill link is already wired up in `_config.yml`.

---

## Running Locally (optional)

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

---

## File Structure

```
.
├── _config.yml          ← Site settings & personal info
├── _data/
│   ├── research.yml     ← Papers
│   └── teaching.yml     ← Courses
├── _includes/
│   └── nav.html         ← Navigation bar
├── _layouts/
│   └── default.html     ← Page template
├── assets/
│   ├── css/main.css     ← All styles
│   └── images/          ← Drop headshot.jpg here
├── index.html           ← Main page content
└── Gemfile              ← Ruby dependencies
```
