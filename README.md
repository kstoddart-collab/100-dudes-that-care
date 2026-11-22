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
- `script.js`: menus, dialogs, FAQs support, and signup delivery and nomination draft downloads.
- `CNAME`: custom domain; keep this file when updating the website.

Changes committed to the selected publishing branch automatically update the site.

## Before launch

Confirm chapter location, meeting dates, organizer contact, nonprofit eligibility, voting policy and quarterly commitment. Contact email remains the reserved placeholder hello@100dudes.example. No payment service is connected. Signup delivery is configured through FormSubmit and is gated until activation and delivery checks pass. Nonprofit nominations still download local drafts only.

The $10,000 quarterly and $40,000 annual figures are illustrative goals based on 100 participants giving $100 quarterly, not historical results.

All branding, copy, illustration and code were created for this project. The giving-circle concept and information structure were inspired by https://www.100womenbeaches.com/. No reference-site assets are included. Fonts are DM Sans and Manrope via Google Fonts, with system fallbacks.

GitHub documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
Custom domain documentation: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Update the quarterly nonprofit

After each member vote, edit `giving-config.js` in GitHub and commit to `main`:

- `recipientName`: chosen nonprofit's name.
- `donationUrl`: verified full HTTPS URL for the nonprofit's own donation page.
- `givingPeriod`: optional quarter or meeting label, such as Q1 2027.
- `description`: optional short explanation of the nonprofit's work.

The Give button and recipient details update automatically after GitHub Pages publishes. Leave `donationUrl` empty to show the recipient-not-announced message. Both a recipient name and a valid HTTPS donation URL are required to activate the external link. Members pay the charity directly; this website does not collect, hold, or forward donations. The charity handles payment and receipts. Do not use an IronMind Advisors payment link.

## Signup delivery

The Count me in form posts to FormSubmit, with kenny@ironmindadvisors.com as the main recipient and louisz@cdzsales.com copied. The signup includes name, email, optional phone and city/neighborhood, and required permission for membership/gathering follow-up. It does not charge or authorize payments.

The mailbox owner must activate FormSubmit before registration is enabled. `signup-config.js` controls the public signup gate. Keep it false until activation and test delivery are verified; then set `window.SIGNUP_ENABLED = true`.

The form retains FormSubmit’s default CAPTCHA and includes a honeypot. Successful form submission returns to `thanks.html`. Nomination forms still download drafts. Signup processing and the provider’s stated 30-day submission retention are disclosed in the privacy dialog. Organizer copies are delivered to email.

For recipient changes, update the form action and hidden _cc field in script.js, activate any new primary inbox and test delivery again before enabling signup.
