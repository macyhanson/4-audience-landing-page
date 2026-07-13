# BrainyAct B2B Landing Page

Static landing page for BrainyAct by Kinuu, targeting health plans, self-insured employers, TPAs, and benefits consultants.

## Structure

    index.html                          single-page site (HTML, CSS, JS inline)
    assets/brainyact-logo.png           nav and footer logo
    assets/hero-brainyact-session.jpg   hero image

## Before going live

Forms are HubSpot embeds (portal 5562675) loaded through `js.hsforms.net/forms/embed/v2.js`. The walkthrough and segment CTAs use form `41360ae6-00bd-454b-9f05-6a37237283d7`; the outcomes sample report CTA uses form `172f270a-5f68-409e-9486-4c4751d1bb81`. Both render into the modal and swap to the thank-you view on submit. HubSpot tracking requires the page to be served over HTTPS from an allowed domain.

Update the canonical URL and Open Graph image URL in `<head>` if the site is served from a domain other than brainyact.com.

## Deploy (GitHub Pages)

Push to the default branch, then enable Pages under Settings, Pages, Deploy from a branch, root folder.
