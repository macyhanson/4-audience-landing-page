# BrainyAct B2B Landing Page

Static site for the four-audience B2B landing page. Deployed with GitHub Pages.

## File structure

Repo root must contain exactly these, and nothing else:

index.html
.nojekyll
README.md
assets/brainyact-logo.png
assets/hero-brainyact-session.jpg

The two asset filenames are hardcoded in index.html. They must match exactly, all lowercase, hyphens not spaces. No "(1)" suffixes.

## Publishing

Settings, then Pages, then Source: Deploy from a branch, branch main, folder / (root).
Interim URL: https://macyhanson.github.io/4-audience-landing-page/

## Moving to brainyact.com

index.html already declares its canonical URL and social preview image as https://brainyact.com/, so no edits are needed when the domain cuts over.

Do the DNS first, then GitHub. At the DNS registrar, create four A records for the apex domain pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, and 185.199.111.153. Add a CNAME record for the www subdomain pointing to macyhanson.github.io.

Once DNS has propagated, go to Settings, then Pages, and enter brainyact.com in the Custom domain field. GitHub creates the CNAME file automatically. Wait for the DNS check to pass, then tick Enforce HTTPS.

Do not add a CNAME file manually before DNS is live. It will break the github.io URL and leave you with no working link in the meantime.
