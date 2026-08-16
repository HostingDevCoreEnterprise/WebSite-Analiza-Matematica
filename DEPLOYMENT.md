# Deployment Guide: Analiza Matematică

This repository contains the static frontend for the Analiza Matematică platform.

## Prerequisites
- A Render account (https://render.com)
- A GitHub/GitLab/Bitbucket repository containing this code
- Access to your domain DNS settings (`analizamatematica.site`)

## Render Configuration
Since this is a simple HTML/CSS/JS frontend without a build step, it should be deployed as a **Static Site** on Render.

1. **Create a New Static Site** in your Render Dashboard.
2. **Connect Repository**: Select the repository that contains this project.
3. **Configuration**:
   - **Name**: `analizamatematica-frontend`
   - **Branch**: `main` (or your primary branch)
   - **Root Directory**: `am site` (or leave blank if the files are in the repository root)
   - **Build Command**: Leave empty.
   - **Publish Directory**: `.` (if `index.html` is in the root directory you specified)
   - **Pull Request Previews**: Optional, but recommended.
4. **Deploy**: Click "Create Static Site".

## DNS Configuration (analizamatematica.site)
Once deployed, Render will provide you with a `.onrender.com` URL. You need to configure your custom domain:

1. In Render, go to your Static Site settings and find the **Custom Domains** section.
2. Add `analizamatematica.site` and `www.analizamatematica.site`.
3. Render will give you specific DNS records to set up. Typically, these are:
   - **CNAME Record**: Name: `www`, Target: `[your-app].onrender.com`
   - **A Record / ALIAS / ANAME**: Name: `@`, Target: IP provided by Render (or ALIAS to `[your-app].onrender.com`).
4. Update your domain registrar's DNS settings with these values.

## SSL / HTTPS
Render automatically provisions a free TLS certificate for your custom domains. Once DNS propagates, your site will be secure (`https://`).

## Post-Deployment Verification
- Visit `https://analizamatematica.site` and ensure it loads.
- Check `https://analizamatematica.site/robots.txt` and `https://analizamatematica.site/sitemap.xml`.
- Ensure there are no broken links and that the developer attribution points to the new domain.
- Submit `sitemap.xml` to Google Search Console to speed up indexing.
