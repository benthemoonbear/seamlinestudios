# Seamline Studio

The website for Seamline Studio: websites, made to measure.

A single hand-written page (`index.html`) with no build step and nothing to install.

## Hosting on Netlify
1. In Netlify, choose **Add new site → Import an existing project → GitHub** and pick this repository.
2. Leave the build command empty. The publish folder is the repository root (set in `netlify.toml`).
3. Click **Deploy**.

## Turning on the enquiry form
The contact form uses Netlify Forms.
1. In Netlify, open the site, go to **Forms** and click **Enable form detection**.
2. Redeploy once (**Deploys → Trigger deploy → Deploy site**).
3. Under **Forms → Form notifications**, add an email notification so each enquiry is emailed to you.

## Adding a project to the portfolio
The projects are written straight into `index.html`, so search engines and AI tools can read them.
1. Save a 1280×800 screenshot of the site's homepage as `img/new-client.jpg`.
2. Make the smaller and lighter copies: `img/new-client-640.jpg`, `img/new-client.webp` and `img/new-client-640.webp` (or ask Claude to do it).
3. In `index.html`, find the comment `PORTFOLIO:`, copy one whole `<article class="project">` block and change the name, link, text, image names and number.
4. To mark unfinished work, keep `<span class="status">In progress</span>` after the number.
5. Commit the change. Netlify publishes it within a minute.

## Files
- `index.html` – the whole site
- `img/` – portfolio screenshots
- `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `site.webmanifest` – browser and home-screen icons
- `og-image.jpg` – the preview image shown when the link is shared
- `llms.txt` – a plain summary of the business for AI search tools
- `404.html` – the page-not-found page
