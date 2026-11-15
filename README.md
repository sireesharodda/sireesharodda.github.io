# Dr. Sireesha Rodda — Academic Portfolio

This is a lightweight, responsive GitHub Pages website. It uses HTML, CSS, JavaScript and one JSON content file. No build tools are required.

## 1. Publish on GitHub Pages
1. Open your personal repository named exactly `sireesharodda.github.io`.
2. Upload **the contents of this folder** to the repository root (not the enclosing folder).
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then Save.
6. Wait for the deployment check to complete. Your site will be at `https://sireesharodda.github.io`.

## 2. Personalise the site
- Replace `assets/images/profile.jpg` with a professional headshot (keep the same filename).
- Add your final CV as `documents/resume.pdf`.
- Edit `content/site-data.json` to update profile details, metrics, publications, talks, courses and awards.
- The GitHub profile is configured as `https://github.com/sireesharodda`. The expected Pages address is `https://sireesharodda.github.io`.

## 3. Add a talk
Create a folder such as `talks/2026/reliable-ml-production/` and upload:
- `photos/` — event photographs
- `presentation.pptx` — slides
- `certificate.pdf` — certificate
- `details.md` — event description

Then add an object to the `talks` array in `content/site-data.json`:

```json
{
  "title": "Designing, Deploying, and Maintaining Reliable Machine Learning Models in Production",
  "date": "15 November 2026",
  "event": "Workshop / FDP name",
  "organizer": "Institution name",
  "role": "Resource Person",
  "description": "Two-hour practical session on production machine learning.",
  "files": [
    {"label": "Presentation", "url": "talks/2026/reliable-ml-production/presentation.pptx"},
    {"label": "Certificate", "url": "talks/2026/reliable-ml-production/certificate.pdf"}
  ]
}
```
Use relative paths exactly as shown. Add photo links in the `files` array if desired.

## 4. Add a publication
Add an object to the `publications` array:

```json
{
  "year": "2026",
  "title": "Full paper title",
  "authors": "Author names",
  "venue": "Journal or conference, volume, issue and pages",
  "links": [
    {"label": "DOI / Publisher", "url": "https://doi.org/..."},
    {"label": "Code", "url": "https://github.com/username/repository"}
  ]
}
```
Only upload or link to the paper PDF when copyright/licensing permits.

## 5. Add teaching resources
Each course has a folder under `content/teaching/`. Add subfolders for:
- `slides/`
- `notes/`
- `lab-manual/`
- `notebooks/`
- `assignments/`
- `projects/`

Upload PDFs, PPTX, DOCX, IPYNB and source code. Add a `README.md` in each course folder with a short course description and links to the resources. Keep filenames short and descriptive.

## 6. Important checks before publishing
- The current profile data reflects the updated CV supplied on 15 November 2026: 43 publications, 341 citations, h-index 9 and i10-index 9. The publication list in this starter package is still a selected subset; add the complete 43-item bibliography before treating the website as a complete publication archive.
- The email address and LinkedIn URL are taken from the supplied resume/profile details. Verify them before publishing.
- Do not publish confidential research data, student personal information, patient-identifiable information, or copyrighted material without permission.
- Large files may exceed GitHub's ordinary file upload limits. For large datasets/videos, link to an approved repository or storage service rather than committing them directly.
