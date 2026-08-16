# Analiza Matematică

Modern educational platform dedicated to **Analiza Matematică**, providing structured learning resources, mathematical materials, and tools for studying the subject.

**Production website:** `https://www.analizamatematica.site`
**Developer:** DevCore Enterprise — `https://www.devcore-enterprise.site`

---

## Overview

This repository contains the frontend for the **Analiza Matematică** educational platform.

The platform was originally created around tutoring activities but has evolved into a complete subject-focused educational resource. The current project is therefore positioned around **Analiza Matematică as a whole**, rather than tutoring specifically.

The application is a static frontend built with HTML, CSS, and JavaScript and does not require a server-side build process.

---

## Technology

* HTML5
* CSS3
* JavaScript
* Static assets
* Render Static Site deployment
* Custom domain: `analizamatematica.site`

---

## Repository Structure

The exact structure may evolve, but the project should generally contain the following:

```text
.
├── index.html
├── assets/
│   ├── css/
│   ├── js/
│   ├── images/
│   └── icons/
├── favicon/
├── robots.txt
├── sitemap.xml
└── README.md
```

---

## Local Development

Because this is a static frontend, no backend server or database is required to run the website locally.

You can open `index.html` directly in a browser for basic testing.

For a more accurate local development environment, use a simple local HTTP server.

For example, with Python:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

If the project is located in a subdirectory, start the server from that directory.

---

## SEO

The website is designed to be search-engine friendly and includes the appropriate technical SEO resources.

### Sitemap

Production sitemap:

```text
https://www.analizamatematica.site/sitemap.xml
```

The sitemap should contain only public, indexable pages.

### Robots

Production robots file:

```text
https://www.analizamatematica.site/robots.txt
```

The `robots.txt` file should allow search engines to crawl public content while avoiding unnecessary internal or non-indexable routes.

### Metadata

Important public pages should have appropriate:

* `<title>`
* meta descriptions
* canonical URLs
* Open Graph metadata
* Twitter/X card metadata where appropriate
* language/locale information
* structured data where applicable

The production canonical domain is:

```text
https://www.analizamatematica.site
```

Development, localhost, preview, or unrelated domains should not be used as production canonical URLs.

---

## Favicon & Branding

The official Analiza Matematică favicon and site icons should be used throughout the application.

The project should use the appropriate:

* browser favicon
* Apple/touch icon where applicable
* web manifest icons where applicable

Default framework or placeholder icons should not be used in production.

---

## Developer Attribution

The official developer website is:

```text
https://www.devcore-enterprise.site
```

The project should reference **DevCore Enterprise** and the domain wherever developer attribution is required.

---

## Google Search Console

The production website can be managed through Google Search Console.

Production domain:

```text
https://www.analizamatematica.site
```

Production sitemap:

```text
https://www.analizamatematica.site/sitemap.xml
```

Google controls the actual indexing process, so submitting a sitemap does not guarantee immediate indexing.

---

## Maintenance

When making future changes:

1. Test changes locally.
2. Verify links and assets.
3. Check SEO metadata for affected pages.
4. Ensure production URLs remain correct.
5. Commit changes to the repository.
6. Push changes to the appropriate branch.

Avoid committing:

* `.env` files containing secrets
* generated build output when unnecessary
* local IDE configuration unless intentionally shared
* temporary files
* personal credentials

---

## License

This is proprietary software owned by the Catedra de Analiză Matematică, Facultatea de Matematică și Informatică, Universitatea din București.

The source code, content, design, and assets may not be copied, modified, distributed, or used without prior written permission.

---

## Project Status

**Production-ready frontend**

Production website:

`https://www.analizamatematica.site`

Developer:

**DevCore Enterprise**

`https://www.devcore-enterprise.site`
