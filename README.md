# I&D Intelligence & Data Pvt. Ltd. — Website

A responsive, static website prepared for deployment to GitHub Pages and the custom domain `iddata.co.in`.

## Before publishing — important

1. **Verify the company email.** The starter site currently uses `contact@iddata.co.in`. Create and test that mailbox first, or replace every occurrence in `index.html`, `privacy.html`, `terms.html`, and `medical-ai-disclaimer.html` with your actual working company email.
2. Review every product description and stage for accuracy. Do not imply that any product is approved, clinically validated, commercially deployed or proven unless you can substantiate the claim.
3. Review the starter Privacy Policy and Terms of Use against your actual practices and applicable law.
4. Add founder names, professional profiles, registered-office details and other company details only after confirming the exact wording you want public.
5. This is a static informational website. It does not include a backend, database, analytics, login, or a working web form.

## Publish with GitHub Pages

1. Create/sign in to a GitHub account.
2. Create a **public** repository named `iddata-website`.
3. Upload all files and folders in this package. `index.html` must be at the repository root.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
6. Wait for the `github.io` website to deploy and test it before changing DNS.

Official guide: https://docs.github.com/en/pages/getting-started-with-github-pages

## Connect the GoDaddy domain

In GitHub, open repository **Settings → Pages → Custom domain**, enter `iddata.co.in`, and save. Follow the verification and DNS instructions shown there.

In GoDaddy, open **My Products → Domains → iddata.co.in → DNS → Add New Record**. For a typical GitHub Pages apex-domain setup, GitHub documents these A records:

| Type | Name | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

For `www`, add a CNAME record with:
- Type: `CNAME`
- Name: `www`
- Value: `YOUR-GITHUB-USERNAME.github.io` (replace with your GitHub username; no `https://` and no path)

**Do not delete MX, SPF, DKIM, DMARC or other email-related records.** If existing A, AAAA or CNAME records conflict with these website records, check the official GitHub instructions before replacing them. Do not change nameservers unless you understand the effect on your email and other services.

Official custom-domain guide: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

After DNS updates propagate, return to GitHub Pages settings and enable **Enforce HTTPS** when the option becomes available. Test both `https://iddata.co.in` and `https://www.iddata.co.in`.

## Files

- `index.html` — homepage
- `privacy.html` — starter privacy policy
- `terms.html` — starter terms of use
- `medical-ai-disclaimer.html` — healthcare AI disclaimer
- `assets/styles.css` — responsive visual styling
- `assets/site.js` — mobile navigation and current-year footer
- `assets/favicon.svg` — site icon
- `robots.txt`, `sitemap.xml` — basic search-engine discovery files

## Google for Startups Cloud Program

Once the website is public, load without a login, has accurate company/product information and works over HTTPS, reply to the existing Google email asking them to reprocess the application. Website availability does not guarantee program acceptance; Google may assess other eligibility requirements.
