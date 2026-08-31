# How this site works

GitHub Pages runs Jekyll for you. Push a markdown file, it becomes a page. There
is no build step and nothing to install.

## Add a page

Make `talks.md` at the top level, starting with this:

    ---
    layout: default
    title: Talks
    ---

Then write markdown below it. To get it into the sidebar, add two lines to the
`nav:` list in `_config.yml`:

      - title: Talks
        url: /talks/

## Add a blog post

Files go in `_posts/` and the name has to be `YYYY-MM-DD-slug.md`. Jekyll refuses
to build if the date is malformed, so copy the pattern exactly:

    _posts/2026-09-14-first-post.md

    ---
    layout: post
    title: What Lorentzian polynomials are for
    ---

    Text here.

The blog page picks it up automatically and the "Nothing here yet" line
disappears on its own.

## Markdown you'll want

    *italic*, **bold**, [link text](https://example.com)

    ## A subheading

    - a list item
    - another

Math is not set up. If you want LaTeX in posts, say so and it's a two-line
addition to the layout (KaTeX or MathJax).

## The red dashed links

Those are placeholders. The `{:.todo}` on the end is what makes them ugly. Fill
in the real address and delete that bit.

## Previewing

You can't open these `.md` files in a browser and see the site; Jekyll has to
build them. Either push and look at the live site a minute later, or install
Ruby and run `bundle exec jekyll serve` locally. Pushing is fine.
