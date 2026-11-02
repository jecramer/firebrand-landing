# James Cramer website

Static website: plain HTML, inline styles, Google Fonts and a small amount of vanilla JavaScript. No build step.

## Structure

- `/` home
- `/approach/`
- `/work/` with case studies at `/work/skunkworks/`, `/work/project-orca/` and `/work/voxelpop/`
- `/engage/` with the enquiry form
- `/writing/` (Signal:Noise index) with four essays at `/writing/<slug>/`
- `/assets/` images

## Deploying

Vercel: import the repository, choose the "Other" framework preset, leave the build command empty and the output directory as the repository root.

Links between pages are relative, so the site also works from a subfolder or GitHub Pages.

## Not yet connected

- The enquiry form on `/engage/` shows a confirmation but does not send or store anything. Connect it to a server-side handler before launch.
- Canonical URLs, `og:url`, `og:image` and `sitemap.xml` need the production domain.
- Essays are static copies of the Substack posts; new posts are added by hand until a CMS is in place.
