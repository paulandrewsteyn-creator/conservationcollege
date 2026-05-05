# Conservation College — landing site

Static, single-page editorial landing site for Course 1 — *Introduction to African Wildlife & Conservation*. Hosted on Netlify, source on GitHub.

## Structure

```
.
├── index.html           Single-file build — HTML, CSS and JS inline.
├── images/              Optimised JPGs (≈1.6 MB total).
│   └── contributors/    Guest expert headshots.
├── netlify.toml         Cache headers, security headers, redirects.
└── README.md
```

## Local preview

Just open `index.html` in your browser — no build step.

## Editing copy

All copy lives in `index.html`. Search for the section comment (e.g. `<!-- HERO -->`, `<!-- PRICING -->`) and edit inline. Push to `main` and Netlify auto-deploys within ~30 seconds.

## Swapping images

1. Drop the new image into `/images/` (kebab-case filename, JPG, ≤ 250 KB ideally).
2. In `index.html`, find the existing path (e.g. `/images/lion-pride.jpg`) and update the `src` / `background-image` to your new file.
3. Commit and push.

## Checkout

Every Enrol button deep-links to Checkout Joy: `https://storefronts.checkoutjoy.com/p/i9pppvjz` with per-button UTMs (`utm_medium=hero`, `pricing_card`, `sticky`, etc.) so you can attribute conversions in analytics.

## Trailer + sample lessons

The Premise trailer and the three Sample Lesson cards open inside an in-page popup modal. Trailer video ID is set in the `data-yt` attribute on `#trailer`; sample IDs live on each `.video-card`'s `href`. Swap a video by changing the YouTube ID in those two places.

## Deploy

Repo is connected to Netlify. Pushing to `main` triggers a build. No build step is required — Netlify just publishes the repo root as-is.
