# Jay Pacamarra — portfolio

Personal website with a project portfolio, blog, learning resources, robotics notes,
Zephyr guides, tips for juniors, and more.

Styled after the [Linux kernel user guide](https://docs.kernel.org/admin-guide/index.html):
documentation-first layout, no build step required.

## Local preview

From the repository root:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000 in your browser.

## Structure

```
index.html          Main hub (table of contents)
_static/style.css   Alabaster-inspired stylesheet
_template.html      Copy-paste starter for new pages
projects/           Portfolio projects
blog/               Blog posts
learning/           Learning resources
robotics/           Robotics notes
zephyr/             Zephyr RTOS notes
juniors/            Tips for early-career engineers
```

## Adding a page

1. Copy `_template.html` to the target path (e.g. `blog/my-post.html`).
2. Update `<title>`, the page `<h1>`, and the body content.
3. Fix relative paths for CSS and sidebar links (`../` per directory level).
4. Mark the current section with `class="current"` on its sidebar `<li>`.
5. Add a link to the new page from the relevant section index and/or `index.html`.

To add a new top-level section, create a folder with `index.html`, add a sidebar
link on every page, and add an H2 section on `index.html`.

## GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Set source to the `master` branch, folder `/ (root)`.
4. The site will be served from `index.html` at the repo root — no extra config needed.

## License

MIT — see [LICENSE](LICENSE).
