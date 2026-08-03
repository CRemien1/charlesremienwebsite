# Charles Remien — Economics Job Market Website

A lightweight static website for Charles Remien's economics job market.

## Pages

- `index.html`: short biography, portrait, and CV download
- `research.html`: job market paper, working papers, projects in early
  development, and additional research experience
- `teaching.html`: courses taught, TA/tutor experience, and teaching materials
- `contact.html`: email, phone, department, profiles, and dissertation
  committee

## Files

- `assets/files/cv.pdf` — CV
- `assets/files/econ103-syllabus.pdf`, `econ191-syllabus.pdf`,
  `econ385-syllabus.pdf` — course syllabi
- `assets/files/econ103-sample-lecture.pdf`, `econ191-sample-lecture.pdf`,
  `econ385-sample-lecture.pdf` — sample lecture slides
- `assets/files/inspector-who-slides.pdf`,
  `assets/files/silver-age-of-mercenaries-slides.pdf` — conference
  presentation slides
- `assets/images/charles-remien-portrait.jpg` — homepage portrait
- `assets/images/halloween-pirate-economics.jpg` — teaching page photo
- `assets/images/profile-placeholder.svg` — unused template leftover, safe to
  delete

To update content, edit the relevant `.html` file directly and add new files
to `assets/files/` or `assets/images/` as needed.

## Publish with GitHub Pages

1. Create a public GitHub repository named `yourusername.github.io`.
2. Upload the contents of this folder to the repository's root.
3. Commit and push the files.
4. Visit `https://yourusername.github.io`.

For a project repository with another name, open the repository's **Settings**,
select **Pages**, and deploy from the `main` branch and root folder.

## Local preview

Open `index.html` directly in a browser, or run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.
