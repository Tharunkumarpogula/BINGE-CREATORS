# BINGE-CREATORS

## Deploy to GitHub Pages

This folder is a static site that works on GitHub Pages.

### Why these changes?
- Asset paths are relative (e.g., `./assets/...`) so the site works under a project subpath like `/your-repo/`.
- Filenames are case-correct for case-sensitive hosting.
- `404.html` mirrors `index.html` so client-side routes work on Pages.

### Quick deploy (project site)
1. Push this folder as the root of `main`.
2. In GitHub: Settings → Pages → Build and deployment:
   - Source: Deploy from a branch
   - Branch: `main` and `/ (root)`
3. Wait for Pages to build, then open the URL it shows.

### CLI steps
```bash
# from this folder
git init
git add .
git commit -m "Deploy to GitHub Pages"
# replace with your repo
git branch -M main
git remote add origin https://github.com/<user>/<repo>.git
git push -u origin main
```

If you use a custom domain, add a `CNAME` file with your domain name.
