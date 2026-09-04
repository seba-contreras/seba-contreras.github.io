# seba-contreras.github.io

Source of [seba-contreras.github.io](https://seba-contreras.github.io/). Jekyll site adapted from
[AcademicPages](https://github.com/academicpages/academicpages.github.io) via the
[Priesemann group website](https://github.com/Priesemann-Group/priesemann-group.github.io) (both MIT).
Pushing to `main` builds and deploys it through GitHub Actions (`.github/workflows/jekyll.yml`);
the repository's Pages source must be set to *GitHub Actions*.

## Where things live

| What | File |
|---|---|
| Name, sidebar bio, profile links, email | `_config.yml` (`author:` block) |
| Profile photo (400×400) | `images/seba_400x400.jpg` |
| CV PDF | `files/CV_SContreras.pdf` |
| Menu | `_data/navigation.yml` |
| Landing page (hero, research themes, latest paper box) | `content/overview.html` |
| Research topics + their selected publications | `_data/research.yml` |
| **All publications** (title, authors, journal, DOI, abstract) | `_data/publications.yml` |
| Collaborators | `_data/collaborations.yml` |
| CV page (positions, education, recognition, editorial, teaching, talks) | `content/cv.html` |
| Contact page | `content/contact.html` |
| Colours (light / dark) | `_sass/theme/_seba_light.scss`, `_sass/theme/_seba_dark.scss` |
| Hero illustration | `img/spreading-network.png` |

## Adding a publication

Add an entry at the top of `_data/publications.yml`:

```yaml
- key: contreras2027something      # unique, used to reference it from research.yml
  title: "Title"
  authors: "First Author, <strong>Seba Contreras</strong><sup>†</sup>, Last Author"
  journal: Journal Name
  year: 2027
  date: '2027-01-15'
  doi: 10.xxxx/yyyy
  type: article                    # article | preprint | chapter
  ref: 12(3), 456                  # volume(issue), pages — optional
  abstract: >-
    Abstract text.
```

`<strong>` highlights your name; `<sup>*</sup>` = equal contribution, `<sup>†</sup>` = corresponding author.
To feature it on the Research page, add its `key` under a topic in `_data/research.yml`.
To feature it on the landing page, edit the "Latest publication" box in `content/overview.html`.

## Local preview

```bash
bundle install
bundle exec jekyll serve      # http://localhost:4000
```
