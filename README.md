# aayushbathija.github.io

Jekyll site. GitHub Pages builds it, so there's nothing to install and no build
step to run.

## Adding a page

1. Make `something.md` in the root with front matter at the top:

       ---
       layout: default
       title: Something
       ---

2. Add it to the `nav:` list in `_config.yml` so it shows in the sidebar.
3. Commit and push.

Front matter is not optional. A `.md` file without it gets served as raw text.

## Adding a post

Put a file in `_posts/` named `YYYY-MM-DD-slug.md`, same front matter plus a
`date:`. It shows up on the Blog page on its own.

## Math

Add `math: true` to a page's front matter. Then `$x^2$` inline, `$$...$$` for
display. KaTeX only loads on pages that ask for it.

## Editing the sidebar text

Name, tagline, and email live in `_config.yml`.
