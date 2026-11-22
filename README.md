# halfapintpub

A personal TTRPG blog built with Hugo (uk/en), styled as a nostalgic glitchy CRT.

## Writing a post

Create a post from the template:

    hugo new posts/my-post.en.md    # or .uk.md

The template (`archetypes/posts.md`) gives every post the same structure:

- Front matter: `hook` (gold lore line under the title), `hero_image` / `hero_alt` /
  `hero_caption` (framed "screenshot" at the top), `player_quote` (dialogue pull-quote),
  `description` (quest-log blurb; falls back to the auto summary). All optional.
- Body shortcodes: `{{< toc >}}…{{< /toc >}}`, `{{< takeaways >}}…{{< /takeaways >}}`,
  `{{< figure src="…" alt="…" caption="…" >}}`, `{{< players >}}…{{< /players >}}`,
  `{{< aside >}}…{{< /aside >}}`.

The article layout renders the front matter blocks (`layouts/partials/crt/article.html`);
component styles live in `static/css/home.css` (`.hook`, `.hero-figure`, `.player-quote`,
`.toc`, `.takeaways`, `.aside-note`).

## Build

    hugo --minify

Deploys to GitHub Pages via `.github/workflows/hugo-build.yml` on push to `main`.
