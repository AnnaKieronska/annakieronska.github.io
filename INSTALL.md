# Anna's Website — Customization Bundle

This zip contains the customized files for Anna Kierońska-Rudek's academic website,
based on the Bryngelson Jekyll template.

## What's inside

- `_config.yml` — site identity (Anna's name, title, ORCID, Scopus, etc.)
- `_data/pi.yml` — education list
- `_data/awards.yml` — awards list
- `_data/grants.yml` — grant list with PI/Co-I roles
- `_data/news.yml` — homepage news items
- `_pages/home.md` — landing page with hero, research chips, bio
- `_pages/research.md` — six research-area cards
- `_pages/teaching.md` — invited lectures + outreach
- `_pages/talks.md` — awards, talks, memberships
- `assets/ref.bib` — all 20 publications in BibTeX
- `.github/workflows/deploy.yml` — workflow triggering on `main` branch

## How to install

From inside `annakieronska.github.io/` (the cloned template folder):

1. **Extract this zip into the folder, overwriting existing files.**
2. **Delete unused template files:**
   ```bash
   rm -f _data/alumni.yml _data/funders.yml _data/people.yml _data/team_members.yml _data/great_mathematicians_and_physicists.csv
   rm -f _pages/team.md _pages/software.md
   rm -f _posts/1961-11-28-space-time.md _posts/2024-05-31-great-mathematicians-and-physicists.md
   rm -f _config_demo.yml
   rm -f papers/*.pdf
   rm -f images/banner.jpg images/headshot.jpg
   rm -rf images/research/
   ```
3. **Add Anna's headshot:** save her photo as `images/headshot.jpg`
4. **Add her CV:** save the PDF as `papers/cv.pdf`
5. **Test locally** (optional but recommended):
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
   Visit http://localhost:4000
6. **Commit and push:**
   ```bash
   git add -A
   git commit -m "Customize site for Anna Kierońska-Rudek"
   git push
   ```
7. **Watch the deploy** on GitHub → Actions tab. Should go green in 2–3 minutes.
   Site live at: https://annakieronska.github.io
