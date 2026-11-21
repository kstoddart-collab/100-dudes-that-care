# 100 Dudes That Care

A responsive community giving website, ready for GitHub Pages at https://100dudesthatcare.org.

## Upload to GitHub

1. Unzip this package. Upload its contents directly to your GitHub repository root, not inside another folder. Include `index.html`, `styles.css`, `script.js`, `CNAME`, and the empty `.nojekyll` file. This README may also be uploaded.
2. Open repository Settings → Pages. Choose Deploy from a branch, main, and /(root), then Save.
3. Confirm Custom domain is `100dudesthatcare.org`. The included CNAME file declares this domain.
4. In GoDaddy DNS, point four A records named @ at 185.199.108.153, 185.199.109.153, 185.199.110.153, and 185.199.111.153. Point the www CNAME at YOUR-USERNAME.github.io (replace with the account or organization owning the repository, without a repository path). Replace conflicting website records, preserve email records, and use these DNS settings at the active DNS provider if nameservers are elsewhere.
5. Once the DNS check passes and the certificate is available, enable Enforce HTTPS in GitHub Pages.

If your upload tool hides `.nojekyll`, create an empty file with that name in GitHub using Add file → Create new file. GitHub Pages uses it to skip Jekyll processing. No build workflow or package installation is needed.

## Edit the website

- `index.html`: page copy, header/footer branding, original SVG illustration, page title and description.
- `styles.css`: layout, colors, fonts, and responsive styles.
- `script.js`: menus, dialogs, FAQs support, and interest/nomination draft downloads.
- `CNAME`: custom domain; keep this file when updating the website.

Changes committed to the selected publishing branch automatically update the site.

## Before launch

Confirm chapter location, meeting dates, organizer contact, nonprofit eligibility, voting policy and quarterly commitment. Contact email remains the reserved placeholder hello@100dudes.example. No payment service is connected. Interest and nomination forms download local drafts only; they do not submit or store information. Connect an approved form service and update the privacy notice before accepting registrations.

The $10,000 quarterly and $40,000 annual figures are illustrative goals based on 100 participants giving $100 quarterly, not historical results.

All branding, copy, illustration and code were created for this project. The giving-circle concept and information structure were inspired by https://www.100womenbeaches.com/. No reference-site assets are included. Fonts are DM Sans and Manrope via Google Fonts, with system fallbacks.

GitHub documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
Custom domain documentation: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
