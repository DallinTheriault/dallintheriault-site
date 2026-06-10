# dallintheriault-site

Personal landing page for Dallin Theriault. One static page that collects the job-hunt
story in a single URL: who I am, why I'm pivoting, and three real projects with repos and
live demos.

Plain HTML and CSS. No backend, no build step, no framework, no tracking. It just serves
`index.html`.

## Structure

```
index.html        the page
styles.css        all styling (one deep-teal accent, mobile-first)
favicon.svg       monogram favicon
images/           screenshot placeholders (swap in real captures, see IMAGES.md)
netlify.toml      Netlify config (publish the repo root, security headers)
IMAGES.md         how to add screenshots + capture specs
```

## Local preview

It's a static file, so just open `index.html` in a browser. Or serve it:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Deploy

Hosted on Netlify, auto-deploying from `main`. There is no build command; Netlify publishes
the repo root as-is.

## Editing checklist

- **LinkedIn URL:** search `index.html` for `data-placeholder="linkedin"` (two spots) and
  paste the profile URL into the `href`.
- **Screenshots:** see `IMAGES.md`.
- **Final domain:** update the `og:url` and `og:image` meta tags in `index.html`.
