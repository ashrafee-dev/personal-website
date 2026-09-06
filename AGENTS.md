# Repository Guide

## Hugo Site

- Use Hugo from the repository root: `hugo server --buildDrafts` for local development and `hugo --minify` for a production build. Hugo writes generated files to `public/`; do not edit them.
- Content pages are in `content/`. The legacy public URLs are intentional: the blog index is `content/blogs.md` at `/blogs.html`, and post URLs are set explicitly in their front matter.
- Keep repeated presentation in `layouts/partials/`. `layouts/_default/baseof.html` owns the shared document shell, header, status bar, and scripts.
- Blog-card metadata belongs in blog front matter. Portfolio projects and skill lists are rendered from `data/projects.yaml` and `data/skills.yaml`, not copied into templates.
- Browser assets belong in `static/`; `static/style.css` and `static/script.js` retain the legacy interactive styling and behavior.
