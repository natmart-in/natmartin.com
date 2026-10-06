# natmartin.com

Personal site, rebuilt from the old Cargo site (natmartin.cargo.site) as plain static HTML.

- Hosted on GitHub Pages from `main` (root). `CNAME` sets the custom domain.
- Both domains use Cloudflare DNS (Sunday's Cloudflare account, free plan), proxied, for HTTPS:
  SSL/TLS mode "Full", Always Use HTTPS on. Nameservers at Namecheap: carl/diva.ns.cloudflare.com.
- natmart.in (and www) 301-redirects to https://natmartin.com keeping the path, via a Cloudflare
  Redirect Rule in the natmart.in zone. The `natmart-in/natmart.in` repo is a fallback redirect page.
- Edit the HTML directly; there is no build step. `style.css` is shared by every page.
- Old Cargo URLs (`/Situator`, `/Mediclude`, `/The-Ant-Calculator`) still work because GitHub Pages serves `Situator.html` at `/Situator`.
- Link arrows sit in a no-wrap span with the last word (`<span class="ext">word</span>`); Safari ignores CSS masks on inline text, so the glyphs are plain SVG backgrounds.
