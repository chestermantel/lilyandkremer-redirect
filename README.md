# lilyandkremer.com → kremerandlily.com redirect

This repo exists only to **redirect the old wedding-site domain to the new one**.
The wedding site was renamed from `lilyandkremer.com` to **kremerandlily.com**
(main repo: `chestermantel/lily-wedding-123`). The old domain is printed on the
Save-the-Dates, so it must keep working.

GitHub Pages serves this repo at `lilyandkremer.com` (via the `CNAME` file). Every
request is bounced to the same path on `https://kremerandlily.com` by `index.html`
(and `404.html`, which catches sub-paths), client-side and path-preserving.

DNS: the `lilyandkremer.com` apex A/AAAA + `www` records stay on Cloudflare,
**DNS-only (grey cloud)**, pointing at GitHub Pages — unchanged from before.
`fantasyflops.lilyandkremer.com` is a separate site and is untouched.
