# GEDA website

The website for the Gulf Economic Development Authority (GEDA), Gulf Province, Papua New Guinea.

It's a simple static website: plain HTML, CSS and a small JavaScript file. It doesn't need a build step, a database or any plugins, so it runs on **GitHub Pages** as it is.

## What's in this folder

| File / folder | What it is |
|---|---|
| `index.html` | The home page, which holds all the content |
| `styles.css` | Colours, fonts and layout, following the GEDA Brand Style Guide |
| `script.js` | The mobile menu, the footer year and the fade-in effect |
| `404.html` | The page people see if a link is broken |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are (don't delete it) |
| `assets/img/` | GEDA logos, the favicon, the phone icon and the social sharing image |
| `assets/fonts/` | The Montserrat and Open Sans font files (stored here, so no Google connection is needed) |
| `assets/docs/` | The GEDA Organisation Profile PDF, linked from the "Download our profile" button |

## How to put it on GitHub Pages

1. Sign in at **github.com** and click **New repository**.
2. Name it `www` (the social sharing tags in `index.html` are set for this name). Set it to **Public** and click **Create repository**.
3. On the new repository page, click **uploading an existing file**.
4. Drag **everything inside this folder** into the upload box, including the `assets` folder and the `.nojekyll` file.
   - Tip: `.nojekyll` is a hidden file. On Windows, turn on *View → Show → Hidden items* in File Explorer so you can see it.
5. Click **Commit changes**.
6. Go to **Settings → Pages**.
7. Under **Build and deployment**, set **Source** to *Deploy from a branch*, **Branch** to `main`, and the folder to `/ (root)`. Click **Save**.
8. Wait 1–2 minutes. Your site will be live at:
   `https://gedapng.org/` (custom domain, see below)

## Social sharing (Open Graph)

The sharing tags in `index.html` point to `https://gedapng.org/`. If the address ever changes (new repository name or your own domain), update the `og:url`, `og:image`, `twitter:image` and `canonical` lines at the top of `index.html`.

To check the preview, paste the site address into Facebook's Sharing Debugger: https://developers.facebook.com/tools/debug/ and click **Scrape Again** after any change.

## Social media links

The social icons in the **Contact** section and the footer link to:

| Platform | Link |
|---|---|
| Facebook | https://www.facebook.com/GEDA.pg |
| YouTube | https://www.youtube.com/@gedapng |
| TikTok | https://www.tiktok.com/@gedapng |
| LinkedIn | https://www.linkedin.com/company/gedapng/ |
| X | https://x.com/Gedapng |

To change a link, search `index.html` for the old address and replace it. Each link appears **three times**: in the Contact section, in the footer, and in the `sameAs` list near the top, which helps Google connect the website to the social pages.

The icons come from Font Awesome Free 6.5.2 (https://fontawesome.com), licence CC BY 4.0. The credit is kept as a comment in `index.html`.

## Custom domain: gedapng.org

The domain **gedapng.org** is registered with **Cloudflare**. The `CNAME` file in this folder tells GitHub Pages to use it, so don't delete it.

**Cloudflare DNS records** (Cloudflare → gedapng.org → DNS → Records). Set every record to **DNS only** (grey cloud):

| Type | Name | Content |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | gedapng.github.io |

**GitHub:** in the `www` repository, go to **Settings → Pages → Custom domain**, enter `gedapng.org`, click **Save**, and then tick **Enforce HTTPS** when it becomes available.
