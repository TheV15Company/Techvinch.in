# TechVinch Amazon Affiliate Store (Starter)

A lightweight, mobile-first static affiliate storefront built with HTML, CSS and JavaScript.

## Preview locally
Open `index.html` in a browser.

## Before publishing
- Replace remaining demo products and sample prices in the `products` array in `index.html`. The featured 360° triangle mop has been added using your supplied product screenshots.
- Add the actual Amazon product URLs with your approved Associates tracking ID.
- Verify prices and availability on Amazon; do not present sample prices as live offers.
- Update contact information and legal pages to match your business.
- Add the required affiliate disclosures and follow the Amazon Associates policies for your marketplace.

## Deploy free with GitHub + Cloudflare Pages
1. Create a GitHub repository (for example `techvinch-store`) and upload `index.html` plus the complete `assets/` folder. The featured mop product images are stored in `assets/`.
2. In Cloudflare dashboard, open Workers & Pages -> Create -> Pages -> Connect to Git.
3. Select the repository. For this plain HTML site, set the build command to `exit 0` (or leave it blank if accepted) and build output directory to `/` or the repository root, as prompted by the current Cloudflare setup.
4. Deploy and test the generated `*.pages.dev` URL.
5. In Cloudflare Pages -> project -> Custom domains, add `techvinch.in` and follow the exact instructions shown. For an apex domain, Cloudflare requires the domain to be set up as a Cloudflare zone and its nameservers pointed to Cloudflare.
6. If DNS is currently managed by another provider, review existing email/MX/TXT records before changing nameservers. Do not delete mail records. Wait for DNS and HTTPS certificate provisioning.

## Notes
- This is a static affiliate showcase. It has no checkout, account system, payment processing, live inventory, or price API.
- Do not commit secrets or passwords to GitHub.
