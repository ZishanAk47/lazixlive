# LAZIXLIVE Website Starter

This is a static preview website. It DOES NOT collect or process payments.

## Before publishing
- Replace the placeholder support email on contact/privacy/terms/refund pages with an email you actively monitor.
- Review all policy text and make sure it matches your real operation.
- Do not activate payments until Razorpay confirms in writing that voluntary viewer contributions/tips for your creator activity are permitted and approves the website.
- Do not put Razorpay Key Secret or webhook secret in HTML/JavaScript.

## Free GitHub Pages hosting
1. Sign in to GitHub and create a public repository named `lazixlive`.
2. Upload the contents of this folder to the repository root.
3. Go to Settings -> Pages.
4. Under Build and deployment, choose Deploy from a branch, select `main` and `/ (root)`, then Save.
5. Your free URL will look like `https://YOUR-USERNAME.github.io/lazixlive/`.

## Razorpay preparation
1. Open Razorpay -> Account & Settings -> Business website details -> Add website/app.
2. Submit the exact published HTTPS URL.
3. Keep the site live and make sure business identity, contact details, policies and payment purpose are consistent.
4. Ask Razorpay support in writing whether this voluntary viewer-support use case is permitted and what documents/category they require.
5. A static site cannot securely create Razorpay orders or verify webhooks. After approval, add a server-side backend for order creation, signature verification and webhook processing. Only verified successful payments should trigger OBS alerts.

## Current limitations
- Donation form is a visual preview only.
- Payment button is intentionally disabled.
- Name/message are not stored and are not verified payment alerts.
- A backend is required for real payments, webhook verification and OBS integration.
