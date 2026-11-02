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
2. Name it, for example `geda-website`. Set it to **Public** and click **Create repository**.
3. On the new repository page, click **uploading an existing file**.
4. Drag **everything inside this folder** into the upload box, including the `assets` folder and the `.nojekyll` file.
   - Tip: `.nojekyll` is a hidden file. On Windows, turn on *View → Show → Hidden items* in File Explorer so you can see it.
5. Click **Commit changes**.
6. Go to **Settings → Pages**.
7. Under **Build and deployment**, set **Source** to *Deploy from a branch*, **Branch** to `main`, and the folder to `/ (root)`. Click **Save**.
8. Wait 1–2 minutes. Your site will be live at:
   `https://YOUR-GITHUB-USERNAME.github.io/geda-website/`

## Using your own domain (optional)

If GEDA buys a domain later (for example `geda.org.pg`):

1. In **Settings → Pages → Custom domain**, type the domain and click **Save**.
2. At the domain provider, add the DNS records that GitHub shows you.
3. Tick **Enforce HTTPS** once it becomes available.

## How to change the content

- To change text, open `index.html` in any text editor (Notepad works) and edit the words between the tags.
  For example, the phone number is in the **Contact** section near the bottom of the file.
- To change colours, edit the colour codes at the top of `styles.css` (in the `:root` section).
- After editing, upload the changed file to GitHub again. The site updates in about a minute.

## Brand rules used

- **Colours:** Leaf Green `#8DC63F`, Charcoal `#3A3A3C`, Slate Grey `#58595B`, White
- **Fonts:** Montserrat (headings) and Open Sans (body text)
- **Logo:** the approved vector files only, never retyped or recoloured
