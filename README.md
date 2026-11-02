# TechFixGuide — free static website starter

A responsive multi-category technology blog starter built with plain HTML, CSS, and JavaScript. It is designed for static hosting on Cloudflare Pages.

## Included
- Responsive home page and navigation
- Six topic categories: Web Development, AI Tools, Free Online Tools, SEO & Marketing, WordPress, E-commerce
- Searchable blog listing and category filters
- Six starter article drafts
- Browser-based word/character counter
- About, Contact, Privacy Policy, Terms, and Disclaimer pages
- `robots.txt`, `sitemap.xml`, favicon, and canonical-tag placeholders

## Before publishing — required edits
1. Search every file for `YOUR-DOMAIN.example` and replace it with your final live website URL (without a trailing slash in the canonical base).
2. In `assets/site.js`, replace `YOUR-CONTACT-EMAIL@example.com` with an email address you monitor.
3. Review and customize Privacy, Terms, Disclaimer, About, and Contact pages. The policy pages are templates, not legal advice.
4. Rewrite and expand starter articles with your own original research, examples, screenshots, and sources before applying for AdSense. These short drafts are not a promise of approval.
5. Update `sitemap.xml` with final canonical URLs. Add article URLs if you later make each article a separate static HTML file.
6. Test every navigation link, search, mobile layout, and contact form after deployment.

## Run locally
Open `index.html` in a browser. For a more realistic local test, serve this folder with any static local server.

## Deploy to Cloudflare Pages
1. Create a GitHub repository and upload the contents of this folder (the files inside `techfixguide`, not the containing parent folder).
2. In Cloudflare, open **Workers & Pages** → **Create** → **Pages** → connect your Git repository.
3. Framework preset: **None**. Build command: leave blank. Build output directory: `/` or the repository root as accepted by the setup screen.
4. Deploy. Cloudflare will provide a `*.pages.dev` URL and HTTPS.
5. Replace placeholder domain references with the deployed URL, commit the changes, and redeploy.
6. Open the site on mobile and test all pages.

## Important functional notes
- Newsletter form is a visual placeholder only. It does not collect or store email addresses. Connect a reputable email service and publish its actual privacy details before enabling subscriptions.
- Contact form opens the visitor's email app using `mailto:`; it is not a server-backed form.
- The category and article listing uses JavaScript, so keep `assets/site.js` available and test that scripts load on the deployed site.
- AdSense approval and earnings are not guaranteed. Follow the current AdSense policies and use original, useful content.
