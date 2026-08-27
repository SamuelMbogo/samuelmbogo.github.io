# samuelmbogo.github.io

Personal site for Samuel Mbogo — Investment Analyst, blended finance & water infrastructure.
Built as a plain HTML/CSS site with no framework or build step.

## What's in this repo

```
index.html            Home
about.html            About + photo + CV downloads
what-i-do.html        Six competency blocks
work.html             Five selected project cards
insights.html         Landing page for insights pieces
services.html         Five advisory service offerings
contact.html          Contact details + CV downloads
insights/             Individual insights pieces
  wasreb-cross-check.html
  moic-over-irr.html
  fund-structure.html
styles.css            Shared stylesheet
favicon.svg           Site favicon
assets/
  sam-mbogo.jpeg      About page photo
cv/
  samuel-mbogo-cv-master.pdf    Full 6-page master CV
  samuel-mbogo-cv-2page.pdf     Trimmed 2-page application CV
```

## Deploying to GitHub Pages (10 minutes, first time)

**Step 1 — Create the repository**

Go to github.com/new (make sure you're signed in as SamuelMbogo).

- Repository name: **`samuelmbogo.github.io`** (this exact name matters — it's what makes the site live at samuelmbogo.github.io)
- Description: "Personal site"
- Public
- Do NOT initialize with a README (we already have files)
- Click "Create repository"

**Step 2 — Upload the files**

On the new empty repo page, click the "uploading an existing file" link (or click "Add file" → "Upload files").

Drag every file and folder from this site folder into the upload area:
- All the `.html` files
- The `styles.css` file
- The `favicon.svg` file
- The `assets/` folder (with the photo inside)
- The `cv/` folder (with both PDFs inside)
- The `insights/` folder (with the three pieces inside)
- This `README.md`

GitHub will accept up to 100 files at once and will preserve the folder structure.

Once uploaded, scroll to the bottom, add a commit message like "Initial site", and click "Commit changes".

**Step 3 — Turn on GitHub Pages**

Go to the repo's Settings tab (top right), then Pages (left sidebar).

- Source: "Deploy from a branch"
- Branch: `main` / `(root)`
- Click Save

Wait about a minute. The Pages settings page will refresh and show a green banner: "Your site is live at https://samuelmbogo.github.io"

**Step 4 — Confirm it works**

Visit https://samuelmbogo.github.io. Click through the pages. Try downloading a CV.

If anything doesn't work, common causes:
- The repo name isn't exactly `samuelmbogo.github.io` (case-sensitive)
- The `index.html` file isn't at the root (make sure it's not inside a subfolder)
- You haven't waited long enough — GitHub Pages takes 30–60 seconds on first deploy

## Updating the site later

Edit any HTML file directly through the GitHub web interface:

1. Go to the repo on github.com
2. Click on the file you want to edit (e.g. `about.html`)
3. Click the pencil icon (top right of the file view) to edit
4. Make your changes
5. Scroll down, add a commit message, click "Commit changes"

Your changes go live within a minute. No local setup needed.

## Adding a new insights piece

1. Copy one of the existing files in `insights/` as a starting point
2. Edit the title, dek, byline, and body
3. Add a new card in `insights.html` that links to it
4. Commit both files

## Notes on the design

- Palette: warm sand background (#F0EDE5), warm near-black text (#23201C), verdigris accent (#4A7C74)
- Type: Instrument Serif for display, IBM Plex Sans for body, IBM Plex Mono for figures inline
- Fonts are loaded from Google Fonts — no local font files needed
- Fully responsive, works on mobile without any extra setup
- All figures in prose (dollar amounts, percentages, page counts) are wrapped in `<span class="fig">…</span>` for the monospace treatment

## Custom domain later (optional, ~$12/year)

If you ever want to move from samuelmbogo.github.io to samuelmbogo.com:

1. Register the domain at any registrar (Namecheap, Cloudflare, Google Domains)
2. In your repo Settings → Pages, add the custom domain
3. Point your domain's DNS at GitHub Pages (they'll show you the exact records)
4. Wait for DNS propagation (a few hours), and GitHub Pages will auto-provision HTTPS

No code changes needed — same repo, same files.
