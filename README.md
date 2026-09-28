# samuelmbogo.github.io

Personal website of Samuel Mbogo, investment analyst, Nairobi. Built with Jekyll and served by GitHub Pages from the `main` branch. Live at https://samuelmbogo.github.io.

## Structure

```
_config.yml          Site settings: name, headline, email, LinkedIn, collections
_data/
  navigation.yml     The menu (edit here to rename or reorder menu items)
_includes/
  header.html        Top bar and menu, shared by every page
  footer.html        Footer, shared by every page
_layouts/
  default.html       The page shell: fonts, stylesheet, link-preview tags
  entry.html         Template for case studies and insights
_work/               One Markdown file per case study
_insights/           One Markdown file per article
tools/               Interactive tools, one HTML file each
assets/
  css/main.css       The whole visual design
  img/               Photo
cv/
  samuel-mbogo-master-cv.pdf
index.html           Home
about.html           About
focus-areas.html     Focus Areas
work.html            Work index (builds itself from _work)
insights.html        Insights index (builds itself from _insights)
tools.html           Tools index
contact.html         Contact
```

## Adding a case study

Create `_work/short-name.md`. The file name becomes the address, for example `/work/short-name/`.

```
---
title: A clear, plain title
summary: One sentence shown on the Work page and on Home.
role: Role, Organisation
period: 2026
focus: Project and infrastructure finance
sector: Sector name
featured: false
order: 25
---

Opening paragraph on why the problem matters.

Paragraph on the client, described without identifying them.

A one-line bridge: what my role was.

What I did.

## What I took from it

One or two sentences.
```

`focus` must be exactly one of: `Project and infrastructure finance`, `Credit and capital structuring`, `Valuation and exits`, `Advisory and assurance`, `Earlier roles`.

## Featuring work

Set `featured: true` on up to six case studies. Featured items appear on Home and at the top of the Work page, ordered by `order` (lowest first). Everything else stays listed under its focus area.

## Adding an insight

Create `_insights/short-name.md`:

```
---
title: The article title
summary: One sentence.
date: 2026-10-15
topic: Credit and capital structuring
---

Article text in plain Markdown.
```

The newest three appear on Home automatically.

## Updating the CV

Export the updated Master CV to PDF, name it exactly `samuel-mbogo-master-cv.pdf`, and drag it onto the `cv` folder to replace the old one. Every link on the site keeps working.

## Hiding something without deleting it

Add `published: false` to the top section of any case study or insight. It disappears from the site until the line is removed.

## Editing workflow

Open the repository on github.com and press the full-stop key to edit in github.dev. Small edits can go straight to `main`: commit and push, and the site rebuilds in one to three minutes (check the Actions tab for a green tick). For larger changes, create a new branch first, build there, and merge through a pull request once it is ready.

## Content rules

- No client or counterparty names. Use the project's code name or a general description.
- Every fact and figure must match the current Master CV.
- Dates on every case study and article.
- No italics and no em dashes.