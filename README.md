# NovaMart storefront starter

A responsive, one-file storefront starter built with HTML, CSS and vanilla JavaScript. Includes product cards, category filters, search, a cart with quantity controls, browser-local cart saving, and WhatsApp order-message generation.

## Before publishing

1. Open `index.html` in a code editor.
2. Search for `const WHATSAPP_NUMBER = "923001234567";` and replace it with your own WhatsApp number in international format using digits only. For Pakistan, use `92` followed by your number without the starting `0`; do not use `+`, spaces or hyphens.
3. Update the `PRODUCTS` array: names, categories, prices, image URLs and image descriptions.
4. Test product filters, the cart, quantity buttons and WhatsApp order text.

## Run locally

Double-click `index.html` to open it in a browser. Internet access is needed for the hosted Unsplash product photos.

## Deploy using GitHub as code storage + Cloudflare Pages as hosting

GitHub Pages' official policy says it is not intended or allowed as free hosting for an online business or an e-commerce site. Keep the source code in GitHub and deploy the storefront through a host that supports your intended use.

1. Create a public GitHub repository, e.g. `novamart-store`.
2. Upload `index.html` and `README.md` to the repository root and commit the changes.
3. Sign in to Cloudflare and open **Workers & Pages**.
4. Choose **Create application → Pages → Connect to Git** (the dashboard wording may vary).
5. Connect GitHub and select your `novamart-store` repository.
6. For this plain HTML site, select no framework / static HTML if prompted. Leave the build command blank and use the repository root (`/`) as the output directory if required.
7. Deploy. Cloudflare will provide a `*.pages.dev` URL. Later pushes to the connected repository can trigger new deployments.

Official docs:
- GitHub Pages limits: https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
- Cloudflare Pages Git integration: https://developers.cloudflare.com/pages/get-started/git-integration/

## Important limitations

- This is a front-end starter, not a complete e-commerce backend.
- WhatsApp order messages are not automatically stored in a database; the customer sends a message and the seller confirms the order.
- No payment details are collected or processed by this site. Do not add card details, API secrets or private customer records to front-end code or a public GitHub repository.
- For online card payments, inventory, admin dashboard, order tracking and customer accounts, integrate a secure backend or use an e-commerce platform/payment provider available in your region.
- Replace demo content and review the terms of your selected hosting provider before using this for a commercial store.
