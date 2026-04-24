# Zhizhen Chen personal website starter

This is a static academic website template. It works with GitHub Pages, Cloudflare Pages, Netlify, Vercel, or any static web host.

## Files

- `index.html` — homepage
- `research.html` — working papers, publications, code
- `writing.html` — notes / blog-style writing
- `bio.html` — bio, education, teaching, contact
- `assets/styles.css` — visual design
- `files/` — place your CV PDF here as `cv.pdf`
- `CNAME.example` — rename to `CNAME` only after your custom domain is ready

## Edit first

Replace these placeholders:

- `your-email@example.com`
- `your-github-username`
- `[your research area]`, `[keyword 1]`, `[keyword 2]`, `[application/domain]`
- paper titles, coauthor names, project links
- add your real CV at `files/cv.pdf`

## Deploy on GitHub Pages

1. Create a GitHub account if you do not have one.
2. Create a repository named exactly `<your-github-username>.github.io`.
3. Upload all files in this folder to the repository root.
4. In GitHub: Settings → Pages → Build and deployment → Source → Deploy from a branch.
5. Select branch `main` and folder `/root`, then Save.
6. Visit `https://<your-github-username>.github.io`.

## Use zhizhenc.us

After you buy `zhizhenc.us`:

1. In GitHub repository: Settings → Pages → Custom domain → enter `zhizhenc.us` → Save.
2. At your domain registrar, add GitHub Pages DNS records:
   - A records for `@` pointing to:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Optional AAAA records for IPv6:
     - `2606:50c0:8000::153`
     - `2606:50c0:8001::153`
     - `2606:50c0:8002::153`
     - `2606:50c0:8003::153`
   - CNAME record for `www` pointing to `<your-github-username>.github.io`.
3. Wait for DNS propagation.
4. In GitHub Pages, enable `Enforce HTTPS` when available.
5. Rename `CNAME.example` to `CNAME` and keep only `zhizhenc.us` inside, or let GitHub create the file automatically when saving the custom domain.

## Optional local editing

Open `index.html` directly in a browser. For a more realistic local preview, use:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.
