
# STR Ops Pack™ – Static Site

A single-file static landing page ready for Vercel or GitHub Pages.

## Deploy to Vercel (Drag & Drop — fastest)

1. Go to https://vercel.com/new
2. Click **Deploy a Static Site** → **Import**.
3. Drag the entire `str-ops-pack-site.zip` (or the unzipped folder) into the window.
4. Name the project (e.g., `str-ops-pack`), then **Deploy**.
5. Your site will be live at a `*.vercel.app` URL. Add a custom domain in the Vercel project settings (optional).

## Deploy to Vercel (GitHub repo)

1. Create a new GitHub repo (public or private).
2. Add these files to the repo root: `index.html`, `README.md`, `vercel.json`.
3. Push to GitHub.
4. Go to https://vercel.com/new → **Continue with GitHub** → select the repo → **Deploy**.

## Deploy to GitHub Pages

1. Create a new repo and upload the files at the root (index.html must be in the root).
2. In repo **Settings → Pages**, set **Source** = `Deploy from a branch`, **Branch** = `main`, folder `/root`.
3. Wait for Pages to build; your site will appear at `https://<username>.github.io/<repo>/`.

## Meta Pixel

Paste the Meta Pixel base snippet into the `<head>` of `index.html` and place your Pixel ID in `fbq('init', 'YOUR_PIXEL_ID')`. Buy buttons have IDs to track clicks:
- `#buy-top`, `#buy-hero`, `#buy-bottom`

Uncomment the `fbq('track', 'AddToCart', ...)` line in the inline script near the bottom.

## Custom Domain (Vercel)

1. In your Vercel project → **Settings → Domains** → **Add** your domain.
2. Follow the DNS instructions (usually a CNAME to `cname.vercel-dns.com`).

## Notes

- This is a pure static site. No build step required.
- Edit copy inside `index.html` and redeploy.
