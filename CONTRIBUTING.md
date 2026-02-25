# Contributing to the MacroEvoEco Website

This site is built with [Quarto](https://quarto.org/) and hosted on GitHub Pages. All team members can suggest changes via pull requests.

## Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/MacroEvoEco/MacroEvoEco.git
   cd MacroEvoEco
   ```

2. Install [Quarto](https://quarto.org/docs/get-started/) if you want to preview locally.

## Making changes

1. **Create a branch** for your changes:
   ```bash
   git checkout -b my-updates
   ```

2. **Edit files** — common tasks:
   - Update your bio or photo on `people.qmd`
   - Add research topics to your page (e.g. `sam-projects.qmd`)
   - Add publications to `publications.qmd`

3. **Preview locally** (optional):
   ```bash
   quarto preview
   ```

4. **Commit and push** your branch:
   ```bash
   git add <files-you-changed>
   git commit -m "Brief description of changes"
   git push -u origin my-updates
   ```

5. **Open a pull request** on GitHub — go to the repo page and click "Compare & pull request".

6. An admin will review and merge your PR. The site rebuilds automatically on merge.

## Branch protection

The `main` branch is protected. You cannot push directly to `main`. All changes must go through a pull request and be approved before merging. Admins can bypass this in urgent cases.

## File guide

| File | What it contains |
|------|-----------------|
| `index.qmd` | Home page |
| `people.qmd` | Team member profiles |
| `research.qmd` | Research themes |
| `projects.qmd` | Funded grants |
| `publications.qmd` | Publication list |
| `students.qmd` | Prospective students info |
| `*-projects.qmd` | Per-person research topics (e.g. `marcel-projects.qmd`) |
| `styles.scss` | Site styling |
| `_quarto.yml` | Site configuration and navbar |
| `images/people/` | Team member photos |

## Adding your photo

Place your photo in `images/people/` and update the image path in `people.qmd` on your team card. Photos are displayed as circles, so square crops work best.

## Questions?

Ask Alex Skeels or open an issue on the repo.
