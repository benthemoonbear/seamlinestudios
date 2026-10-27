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
1. Save a 1280×800 screenshot of the site's homepage into `img/` (for example `img/new-client.jpg`).
2. In `index.html`, find `const PROJECTS = [` and copy one of the project blocks:
   ```js
   {
     name: "New Client",
     type: "What the business does",
     url: "https://example.co.uk",
     summary: "One or two sentences about the project.",
     image: "img/new-client.jpg"
   }
   ```
3. Commit the change. Netlify publishes it within a minute.

## Files
- `index.html` – the whole site
- `img/` – portfolio screenshots
- `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `site.webmanifest` – browser and home-screen icons
- `og-image.png` – the preview image shown when the link is shared
- `404.html` – the page-not-found page
