# gh-deployment-workflow

This repository demonstrates how to use **GitHub Actions** to automatically deploy changes in the `index.html` file to **GitHub Pages**.

Whenever `index.html` is updated in the `main` branch, a workflow triggers to update the live website hosted at GitHub Pages.

---

## Files

- `index.html` – The main HTML file for the website.
- `.github/workflows/deploy.yml` – GitHub Actions workflow that deploys `index.html` to the `gh-pages` branch.
- `README.md` – This file, explaining the project.

---

## Workflow

- The workflow triggers **only when `index.html` is modified** on the `main` branch.
- It uses `peaceiris/actions-gh-pages` to deploy the file to the `gh-pages` branch.
- The website is automatically updated at:  
  [https://sa8aa.github.io/gh-deployment-workflow/](https://sa8aa.github.io/gh-deployment-workflow/)

---

## Usage

1. Make changes to `index.html` in the `main` branch.
2. Push the changes to GitHub.
3. The workflow will automatically deploy the updated file to the GitHub Pages site.

---

## Notes

- **Do not modify the `gh-pages` branch manually** — it is managed automatically by the workflow.
- Only changes in `index.html` in `main` trigger deployment.
