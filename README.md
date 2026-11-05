# SCW / Sean C. Wayda — Multi-Industry Career Portfolio

## What's included
Eleven responsive HTML pages: Home, Projects, Construction Leadership, Preconstruction & Contracts, Retail, Ventures, Consulting, Career, Contact, Project Detail, and 404. The Projects page supports live search, category filters, and project detail pages. Drybar project photographs appear in the gallery with explicit attribution/rights warnings; other projects show labeled architectural diagrams rather than fake project photographs.

## Preview locally
- Unzip the whole package, preserving the `assets/` folder.
- Open `index.html` in Chrome/Edge, or run `python -m http.server 8000` inside this folder then browse to `http://localhost:8000`.
- The site is static and does not require API keys, a paid website builder, or a backend to preview.

## Edit project content
- Edit `site-data.json` (human-readable source data).
- Update `assets/data.js` with `window.SCW_DATA = <contents of site-data.json>;` so the browser can open the site directly from disk. When maintaining via a script, regenerate this file from JSON. Edit only data you can substantiate.
- To add another project, duplicate a record in `site-data.json` with a **unique** `slug`. The project link is `project.html?project=the-slug`.
- For photographs, add compressed JPG/WebP under `assets/photos/`, set a project's `photo` property to `assets/photos/filename.webp`, and add file names to `gallery`. Obtain publication permission first.
- Do not reuse Drybar photos for other projects. The location represented by the Drybar folder remains unverified.
- Update email/LinkedIn in `contact.html`, `assets/site.js`, and the content JSON as needed.
- HTML pages are editable independently; CSS is `assets/style.css`.

## Publish free
Use Cloudflare Pages or Netlify for static hosting within their current free limits; upload the unzipped contents, NOT the ZIP itself when the platform expects a project folder. You can also commit the files to a GitHub repository and deploy it. Do not mistake a local file preview for a deployed website.

## Scope and safeguards
- This is a **static website**. The contact form creates a message in the visitor's email application; it does not send or store it.
- There is **no authentication, upload dashboard, database, or Supabase connection** in this package. Do not call it a completed backend.
- Recent roles and current responsibilities are based on the supplied career description and prior résumé; previous company project archives may not establish individual credit.
- Before public publication, confirm actual project-specific roles, photography licenses, named clients, dates, and employer disclosure permissions.
- Do not expose original estimates, pricing, building plans, confidential business folders, tenant names, or contract redlines.
- Startups are clearly labeled initiatives/development concepts, not revenue claims.

## Important source record constraints
- Drybar: Scottsdale and Camelback locations are documented, but the seven images in the `Drybar` folder are not tied to one address by verified metadata.
- Which Wich, Power Ranch, multifamily townhomes, Hot N Juicy: company-level records, with specific personal contributions needing confirmation.
- Wessman: all source budgets are confidential and deliberately not reproduced.
- Blind Ideas: individual client details are anonymized. 150–680 units is development scale, not the size of the awarded specialty trade package.
- Some dates/titles in older company marketing records conflict with later résumé chronologies. This site preserves current résumé dates and adds qualifiers for unverified earlier roles.

## Next release
The next phase should add backend functionality using your existing Supabase project with database-level owner authorization and Row-Level Security, private document storage, and a persistent photo uploader. Do not enable a fake demonstration login and publish it as secure.
