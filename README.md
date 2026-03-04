# PPBootcamp2026
Designing High‑Impact Prompts &amp; Workflows with Microsoft 365 Copilot and GitHub Copilot

## Markdown Content Management – Folder Structure

This project uses the following folder structure for managing Markdown content:

```
PPBootcamp2026/
├── content/
│   ├── posts/          # Blog posts and articles (YYYY-MM-DD-title.md)
│   └── pages/          # Static pages (about.md, contact.md, etc.)
├── templates/
│   ├── post.md         # Template for new blog posts
│   └── page.md         # Template for new static pages
├── assets/
│   ├── images/         # Image files referenced in Markdown content
│   └── css/            # Stylesheets for rendered Markdown
├── config/
│   └── site.json       # Site-wide configuration (title, description, URL)
└── scripts/            # Build and utility scripts
```

### Getting Started

1. **Create a new post** – Copy `templates/post.md` to `content/posts/YYYY-MM-DD-title.md` and fill in the content.
2. **Create a new page** – Copy `templates/page.md` to `content/pages/page-name.md` and fill in the content.
3. **Update site settings** – Edit `config/site.json` with your site details.
4. **Add images** – Place image files in `assets/images/` and reference them in Markdown using relative paths.
