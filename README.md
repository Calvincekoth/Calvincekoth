# Calvince Okoth: Data Analyst Portfolio

A single-page portfolio built with plain HTML, CSS and JavaScript. No build step or installs needed.

## Project structure
```
index.html        the whole site (content, styles, scripts)
images/           profile photo and Night of Code photos
videos/           put Night of Code videos here
README.md
```

## Run it on your PC
1. Install VS Code (https://code.visualstudio.com) and Git (https://git-scm.com).
2. Open this folder in VS Code and double-click `index.html` to view it in your browser.
   (Optional: install the "Live Server" extension and click "Go Live" to refresh as you type.)

## Put it on GitHub Pages (free)
1. Create a GitHub account, then a new repository named `calvincekoth.github.io` (public).
2. In the project folder, run:
   ```
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Calvincekoth/calvincekoth.github.io.git
   git push -u origin main
   ```
3. On GitHub: Settings > Pages > Source: "Deploy from a branch" > Branch: `main` / root > Save.
4. After a minute your site is live at `https://calvincekoth.github.io`.

## Update the site later
- Edit `index.html`, then run `git add . && git commit -m "Update" && git push`. The site updates by itself.
- Add a project: copy an existing block inside `<section id="experience">` and change the text and links.
- Add a photo: put it in `images/` and copy a `<figure>` in the Networking gallery.
- Add a video: put the file in `videos/` (keep each under 100 MB for GitHub) and add a line to the `VIDEOS` list near the bottom of `index.html`. For long recordings, upload to YouTube and link to it instead.

## Custom domain (optional)
Buy a domain (about KSh 1,500 to 2,500 a year). In GitHub: Settings > Pages > Custom domain, then add the DNS records your registrar needs. Tick "Enforce HTTPS".

## Vercel or Netlify instead
Import the GitHub repository, leave the build settings empty, and deploy.
