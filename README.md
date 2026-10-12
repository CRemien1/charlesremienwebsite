# Charles Remien — Economics Job Market Website

A lightweight static website for Charles Remien's economics job market.

## Pages

- `index.html`: short biography, portrait, recent news, upcoming
  presentations, and CV download
- `research.html`: job market paper, articles accepted for publication,
  working papers, projects in early development, and additional research
  experience
- `teaching.html`: courses taught (Econ 103, 191, 385, 410), TA/tutor
  experience, and teaching materials
- `contact.html`: email, phone, department, profiles, dissertation
  committee, and job-market availability

## Files

- `CNAME` — custom domain (`charlesremien.com`); do not delete
- `assets/files/cv.pdf` — CV
- `assets/files/econ103-syllabus.pdf`, `econ191-syllabus.pdf`,
  `econ385-syllabus.pdf`, `econ410-syllabus.pdf` — course syllabi
- `assets/files/econ103-sample-lecture.pdf`, `econ191-sample-lecture.pdf`,
  `econ385-sample-lecture.pdf`, `econ410-sample-lecture.pdf` — sample lecture
  slides
- `assets/files/cuba-slides.pdf`, `inspector-who-slides.pdf`,
  `silver-age-of-mercenaries-slides.pdf` — conference presentation slides
- `assets/images/charles-remien-portrait.jpg` — homepage portrait
- `assets/images/halloween-pirate-economics.jpg` — teaching page photo
- `assets/images/profile-placeholder.svg`, `assets/files/PLACE_FILES_HERE.txt`
  — unused template leftovers, safe to delete

To update content, edit the relevant `.html` file directly and add new files
to `assets/files/` or `assets/images/` as needed. Replacing a PDF (for
example `cv.pdf`) keeps the same link working; visitors may need a hard
refresh to see a cached older copy.

## Hosting and deployment

- Hosted free on GitHub Pages from the `main` branch (root folder) of
  `github.com/CRemien1/charlesremienwebsite`.
- The custom domain `charlesremien.com` is registered at Cloudflare. DNS has
  four `A` records for `@` pointing to GitHub Pages
  (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`,
  `185.199.111.153`) and a `CNAME` for `www` pointing to
  `cremien1.github.io`. All records are set to "DNS only" (proxy off) so
  GitHub can issue the HTTPS certificate.
- Changes go live only after they are committed and pushed:

  ```bash
  git add -A
  git commit -m "describe the change"
  git push
  ```

  GitHub Pages rebuilds within a minute or two; PDFs can take a little
  longer to refresh.

## Upkeep checklist

- After a conference ends, remove it from "Upcoming presentations" on the
  homepage and add a "Presented at…" note to that paper's line on
  `research.html`.
- When the accepted *Journal of Population Research* paper is published,
  rename its section to "Publications" and add the journal link and DOI.
- Keep "Recent news" short and dated, newest first.

## Local preview

Open `index.html` directly in a browser. If Python is installed, you can also
run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.
