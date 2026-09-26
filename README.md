# Portfolio site — setup

Five pages: `index.html` (home), `paintings.html`, `moving-image.html`, `curator.html`, `about.html`, sharing one `style.css`.

## Swap in your content
- Replace each `<div class="frame">Image placeholder</div>` with a real image:
  ```html
  <div class="frame">
    <img src="images/your-file.jpg" alt="Description" style="width:100%;height:100%;object-fit:cover;">
  </div>
  ```
- Put your image files in the `images/` folder.
- Edit titles, mediums, dimensions, years, bio text, and the email address directly in the HTML files.
- On `curator.html`, each `.row` is one project/screening entry — duplicate the block to add more.

## Put it on GitHub Pages

1. Create a new repo on GitHub named exactly: `yourusername.github.io`
2. Upload all the files (`index.html`, `paintings.html`, `moving-image.html`, `curator.html`, `about.html`, `style.css`, `images/`) — drag-and-drop on GitHub's website, or with git:
   ```
   git init
   git add .
   git commit -m "first version"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source → main branch** → Save.
4. Live at `https://yourusername.github.io` within a minute or two.

## Optional: custom domain
1. Buy a domain (Cloudflare Registrar or Namecheap — no markup, cheap).
2. Add a file named `CNAME` (no extension) to the repo root containing just your domain.
3. At your registrar, point DNS to GitHub Pages (GitHub's docs list the exact A records + CNAME for `www`).
