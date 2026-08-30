# jihyun-home

Academic website for **Jihyun Lee, Ph.D.**, Assistant Professor, Department of
Educational Psychology, University of North Texas.

Built with Jekyll + the [Academic Pages](https://github.com/academicpages/academicpages.github.io)
template and hosted for free on GitHub Pages. GitHub builds and deploys the site
automatically on every push to `main` — no local build step required.

## Site structure

| Page | File |
|---|---|
| Home / bio | `_pages/about.md` |
| Education | `_pages/education.md` |
| Professional Position | `_pages/position.md` |
| Publications (Methodological / Applied / In Progress / Invited) | `_publications/*.md` |
| Presentations | `_talks/*.md` |
| Instructional Activities | `_pages/instructional-activities.md` |
| Professional Journal Activities | `_pages/journal-activities.md` |
| Professional Membership | `_pages/membership.md` |
| Contact | `_pages/contact.md` |
| CV | `_pages/cv.md`, PDF at `files/Lee_CV.pdf` |

Site-wide settings (name, title, bio, email) are in `_config.yml`. The top navigation
order is controlled by `_data/navigation.yml`.

## Making updates

**Add a new publication:** create a new file in `_publications/`, following the pattern
of an existing one (front matter needs `title`, `collection: publications`, `category`
— one of `methodological`, `applied`, `in_progress`, or `invited` — `permalink`, `date`,
`venue`, and `citation`). Commit and push to `main`.

**Add a new presentation:** same idea, in `_talks/` (`collection: talks`, plus `type`,
`venue`, `location`, `date`).

**Update the CV:** replace `files/Lee_CV.pdf` with the new file, keeping the exact same
filename so the download link on the CV page never breaks.

**Edit any other section:** edit the corresponding Markdown file in `_pages/` directly.

After any edit, commit and push to `main` — GitHub Pages rebuilds the live site
automatically within a minute or two.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000/jihyun-home/`.

## Deployment

GitHub Pages should be configured under **Settings → Pages** to build from the `main`
branch, root folder. The live site is served at `https://jihyunl.github.io/jihyun-home/`.
