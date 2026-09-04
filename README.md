# seba-contreras.github.io

Source of [seba-contreras.github.io](https://seba-contreras.github.io/), built with [Hugo Blox](https://hugoblox.com/) (Academic CV template, the successor of Wowchemy/Academic).

The source lives on `main` in this repo; GitHub Actions builds the site and deploys it to GitHub Pages on every push. **Do not commit the `public/` folder.**

## Editing the site

| What | Where |
|---|---|
| Bio, role, affiliations, links, education, experience, awards, skills | `data/authors/me.yaml` |
| Profile photo | `assets/media/authors/me.jpg` |
| CV PDF | `static/uploads/CV_SContreras.pdf` |
| Homepage sections (order, titles, contact block) | `content/_index.md` |
| CV page sections | `content/experience.md` |
| Publications | `content/publications/<key>/index.md` (+ optional `featured.jpg`, `cite.bib`) |
| Collaborators | `content/collaborators/<slug>/index.md` (+ `featured.jpg`) |
| Menu | `config/_default/menus.yaml` |
| Colours, fonts, search, analytics | `config/_default/params.yaml` |
| Hugo version used by CI | `hugoblox.yaml` (`build.hugo_version`) |

### Adding publications from BibTeX

Put BibTeX entries in a file named `publications.bib` at the repo root and push. The
`Import Publications From Bibtex` workflow converts them into `content/publications/<key>/index.md`
and opens a pull request for you to review and merge. You can also run it manually from the
Actions tab, or locally:

```bash
pip install academic
academic import publications.bib content/publications/ --compact
```

Set `featured: true` in a publication's front matter to show it in the *Featured Publications* grid;
drop a `featured.jpg` next to its `index.md` to give the card an image.

## Local preview

```bash
# once: Hugo extended (version in hugoblox.yaml), Go, Node 22, pnpm
pnpm install
hugo server -D
```

## Deployment

`.github/workflows/deploy.yml` builds and deploys on push to `main`. The repository setting
**Settings → Pages → Build and deployment → Source** must be **GitHub Actions** (not "Deploy from a branch").
