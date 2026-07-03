# rm.rar portfolio — how to edit & host it (free, no Netlify)

## What's in here
- `index.html` — the whole site (one file, no build step, no dependencies to install)
- `assets/avatar.png` — your photo

## Editing the content
Open `index.html` in any text editor (Notepad, VS Code, etc.) and look for these spots:

- **Bio text** — search for `<p class="bio">` and rewrite the sentence inside it.
- **Links** — search for `<div class="links"` and edit any `href="..."` to point wherever you want, or delete a whole `<a class="pill">...</a>` block to remove a link.
- **Projects** — search for `id="projects"` and edit/duplicate the `<div class="card">` blocks. Replace the "Coming soon" tag and description once you have something real.
- **Edits section** — same idea, under `id="edits"`, for linking your best TikTok/YouTube edits.
- **Accent color** — near the top of the file under `:root`, change the hex value next to `--accent` to any color you want.

## Hosting it for free (not Netlify)

### Option A — GitHub Pages (recommended, free forever, your own `username.github.io` URL)
1. Create a free GitHub account if you don't have one: https://github.com/signup
2. Create a new repository, name it anything (e.g. `portfolio`), make it Public.
3. Upload `index.html` and the `assets` folder into that repo (drag-and-drop works on github.com, or use `git push` if you're comfortable with git).
4. Go to the repo's Settings → Pages → under "Build and deployment" set Source to "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
5. GitHub gives you a live URL in a minute or two, usually `https://yourusername.github.io/portfolio/`.

### Option B — Vercel (also free, slightly faster setup if you're not comfortable with git)
1. Sign up at https://vercel.com with GitHub.
2. Import the same repo, or use their drag-and-drop deploy for a static folder.
3. You get a free `yourproject.vercel.app` URL.

### Option C — Cloudflare Pages (also free)
Same idea as Vercel — connect a GitHub repo or drag-and-drop the folder at https://pages.cloudflare.com.

Any of these are genuinely free, no card required, and none of them is Netlify.

## A custom domain later
If you ever want something like `rmrar.com` instead of a `.github.io`/`.vercel.app` subdomain, you'd buy a domain (a few dollars/year from a registrar like Porkbun or Namecheap) and point it at whichever host you pick — happy to walk through that when you're there.
