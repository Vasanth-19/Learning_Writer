# The Commons

A Medium-style publication where writers contribute via pull requests instead of accounts. Built with Jekyll, hosted free on GitHub Pages.

## Setup

1. **Create a new GitHub repo** (public), then push this project to it:

   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repo → **Settings** → **Pages**
   - Under "Build and deployment", set Source to **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)`
   - Save. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/` within a few minutes.

3. **Update the config**

   In `_config.yml`, set:
   ```yaml
   url: "https://YOUR_USERNAME.github.io"
   baseurl: "/YOUR_REPO"
   ```

   Then find-and-replace `YOUR_USERNAME/YOUR_REPO` across `_layouts/default.html`, `about.md`, and `README.md` with your actual GitHub username and repo name.

4. **Optional: custom domain**
   Add a `CNAME` file with your domain, and point your DNS at GitHub Pages (see [GitHub's guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)).

## Local development

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`.

## How writers contribute

See [CONTRIBUTING.md](CONTRIBUTING.md) — short version: fork, add a Markdown file to `_posts/`, open a pull request.

## Structure

```
_config.yml          site settings
_layouts/            page templates (default, post)
_posts/              all articles (one .md file each)
assets/css/          styling
index.html           homepage post feed
about.md             about page
CONTRIBUTING.md       writer instructions
```

## Customizing

- **Colors/fonts**: edit `assets/css/style.css` (CSS variables at the top)
- **Site name/description**: edit `_config.yml`
- **Pagination**: change `paginate: 6` in `_config.yml`
