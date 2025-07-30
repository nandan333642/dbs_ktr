# dbs_ktr

Database and KTR-related project.

## Static site

A simple static site lives in the `site/` directory. It contains plain HTML, CSS and JavaScript files.

### Building locally

To preview the site locally, serve the `site/` directory with any static file server. For example using Python:

```bash
python3 -m http.server --directory site 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

### Deployment

A GitHub Actions workflow located at `.github/workflows/deploy.yml` builds the contents of `site/` and deploys them to GitHub Pages whenever changes are pushed to the `main` branch.

Once the workflow completes, the site will be available at:

```
https://<your-github-username>.github.io/dbs_ktr/
```

Replace `<your-github-username>` with your GitHub account name.
