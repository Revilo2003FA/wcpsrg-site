# Putting the site online with GitHub Pages

GitHub Pages is free, hosts static HTML sites forever, and gives the
site a URL anyone can visit. It's the easiest option when you don't
want university IT involved. Total time: about 20 minutes the first
time.

---

## Part 1 — Create a GitHub account (skip if you have one)

1. Go to https://github.com/signup
2. Sign up with your school or personal email.
3. Confirm your email.

## Part 2 — Create the repository

1. Click the **+** in the top right → **New repository**.
2. Name it something like `wcpsrg-site` (or anything — it doesn't have
   to match your domain).
3. Set it to **Public** (required for free GitHub Pages).
4. Check **Add a README file**.
5. Click **Create repository**.

## Part 3 — Upload the website files

1. On the repository page, click **Add file** → **Upload files**.
2. Drag the entire contents of your site folder into the box:
   - `index.html`
   - the `papers/` folder (with both `.html` files inside)
   - the `images/` folder (add your campus photos here first)
   - `HOW-TO-EDIT.md` (optional — nice to keep)
3. At the bottom, write "Initial upload" and click **Commit changes**.

## Part 4 — Turn on GitHub Pages

1. In the repository, click **Settings** (top tab).
2. In the left sidebar, click **Pages**.
3. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main` · `/ (root)`
   - Click **Save**.
4. Wait about 1–2 minutes. Refresh the page.
5. You'll see a green box with your live URL, something like:

   ```
   https://yourusername.github.io/wcpsrg-site/
   ```

Share that URL. The site is live.

---

## Part 5 — (Later) Add a custom domain

A custom domain is optional. The GitHub URL works forever.

If you want something like `wcpsrg.org`:

1. Buy the domain at **Cloudflare Registrar** (cheapest, no markup —
   https://www.cloudflare.com/products/registrar/) or **Namecheap**.
   A `.org` runs about $10–15/year.
2. In your GitHub repo: **Settings** → **Pages** → **Custom domain**
   box. Type your domain (e.g. `wcpsrg.org`) and **Save**.
3. GitHub will show you DNS records to add. Go back to your domain
   registrar, find DNS settings, and add the records GitHub listed.
4. Wait a few minutes to a few hours for DNS to propagate.
5. Back in GitHub Pages settings, check **Enforce HTTPS**.

That's it — your site is at your custom domain.

---

## Updating the site later

Two ways:

**On GitHub (no software needed):**
- Open the file in your repo (e.g. `index.html`)
- Click the pencil icon, edit, scroll down, click **Commit changes**
- Site updates in about a minute

**From your computer:**
- Download the repo (Code → Download ZIP) or install GitHub Desktop
- Edit files in a text editor, then upload the changed files

See `HOW-TO-EDIT.md` for the specific lines to change for common edits.

---

## Alternative: Netlify (also free, drag-and-drop)

If GitHub feels like overkill, Netlify lets you just drag a folder
onto their site:

1. Go to https://app.netlify.com/drop
2. Sign up with GitHub or email.
3. Drag your whole site folder onto the page.
4. Done — you get a URL like `amazing-curie-abc123.netlify.app`.
5. You can rename it in Site settings to something like
   `wcpsrg.netlify.app`.

The downside vs. GitHub Pages: updating the site means dragging the
folder again each time. Fine for a simple site that rarely changes.
