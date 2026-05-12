PawnVision OS is now prepared for Cloudflare Pages.

Project type:
- static site

Cloudflare Pages settings:
- Framework preset: `None`
- Build command: leave blank
- Build output directory: `.`
- Root directory: leave blank unless you import a monorepo

Primary domain:
- `pawnvision-os.com`

Suggested domain structure:
- `pawnvision-os.com` = public site
- `www.pawnvision-os.com` = redirect to primary domain
- `app.pawnvision-os.com` = future broker/dashboard app

Files added for Cloudflare:
- `wrangler.toml`
- `_redirects`

Recommended Cloudflare setup:
1. Create a new Cloudflare Pages project.
2. Connect GitHub repo: `bbart420247/pawnvision-os`
3. Use the settings above.
4. Add the custom domains:
   - `pawnvision-os.com`
   - `www.pawnvision-os.com`
5. Configure `www` to redirect to the primary domain.

Notes:
- The site is static, so no Node build step is required.
- The dashboard and public site remain in the same repo for now.
- If the future broker app becomes dynamic, move it to `app.pawnvision-os.com` separately.
