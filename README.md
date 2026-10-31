# NGHIA DNS PRO website

## Deploy
Upload these files to the root of your GitHub Pages repository:
- `index.html`
- `NGHIA_DNS_PRO.mobileconfig`

Then open repository Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.

The website download button serves `NGHIA_DNS_PRO.mobileconfig`.

## DNS endpoint note
The profile retains the Cloudflare Gateway DoH endpoint from the supplied original profile:
`https://bxb9l1j9j0.cloudflare-gateway.com/dns-query`

The endpoint and filtering policy are controlled by the Cloudflare Gateway account owner. The NGHIA DNS PRO label does not mean this is an independently operated DNS resolver.
