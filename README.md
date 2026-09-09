# Deploy to GitHub Pages

This repository contains a single static HTML file `swsh.html`. The included GitHub Actions workflow will publish the repository root to GitHub Pages whenever you push to the `main` branch.

Steps to publish:

1. Create a new repository on GitHub (public recommended).
2. In your local repo (if not already a git repo):

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin git@github.com:<your-username>/<your-repo>.git
git push -u origin main
```

3. The workflow will run on push and publish the contents to the `gh-pages` branch. Your site will be available at:

```
https://<your-username>.github.io/<your-repo>/
```

Notes:
- If your default branch is not `main`, update `.github/workflows/gh-pages.yml` accordingly.
- To use a custom domain, add a `CNAME` file to the repository root containing your domain.
