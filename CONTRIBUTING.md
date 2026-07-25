# Writing for The Commons

No account needed — you publish by opening a pull request. Here's the full process.

## 1. Fork the repository

Click **Fork** in the top right of the GitHub repo page. This creates your own copy.

## 2. Add your post

In your fork, create a new file inside `_posts/` named:

```
YYYY-MM-DD-your-post-title.md
```

Example: `2026-07-25-why-i-quit-my-job.md`

## 3. Fill in the front matter

Every post starts with this block at the very top:

```yaml
---
title: "Your Post Title"
subtitle: "One sentence that makes someone want to click."
author: "Your Name"
author_avatar: "/assets/images/default-avatar.svg"  # or a link to your own photo
tags: [tag-one, tag-two]
---
```

Then write your post in Markdown underneath.

**Optional: use your own avatar.** Upload a square image to `assets/images/authors/yourname.jpg` and point `author_avatar` at it — e.g. `/assets/images/authors/yourname.jpg`.

## 4. Preview locally (optional but recommended)

If you have Ruby installed:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000` to see your post rendered before submitting.

## 5. Open a pull request

Push your branch and open a PR against `main`. In the description, add a one-line summary of what you wrote. A maintainer will review for formatting and clarity, then merge.

Once merged, GitHub Pages rebuilds the site automatically and your post goes live — usually within a minute or two.

## Writing guidelines

- Markdown only — no raw HTML unless necessary
- Keep images under 1MB; link to external hosting for anything larger
- No plagiarized or AI-generated-without-disclosure content
- Be kind. Disagreement is fine; hostility isn't.

## Editing an existing post

Open a PR that modifies the relevant file in `_posts/`. Only the original author or a maintainer should edit a post's core content.
