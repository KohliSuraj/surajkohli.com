# Infrastructure

How surajkohli.com is set up, and why.

## Domain

- Registered with **Spaceship**.
- DNS is managed in **Spaceship**.
- Why: GitHub Pages works with any DNS provider, so there was no need to move DNS anywhere else.

## Website

- Hosted on **GitHub Pages**.
- Every push to `main` deploys the site through `.github/workflows/pages.yml`.
- The `CNAME` file sets the custom domain to `surajkohli.com`.
- `www.surajkohli.com` redirects to `surajkohli.com`.

## Analytics

- **Cloudflare Web Analytics**, added by hand as a script tag in `index.html`.
- Why by hand: traffic does not pass through Cloudflare, so Cloudflare cannot add it automatically.

## Chatbot

- The backend lives in a separate repo, `KohliSuraj/career-chatbot`.
- Hosted on the **Northflank** free sandbox as one always-on container.
- Address: `https://p01--career-chatbot-backend--zmby9qq4v8rg.code.run` (no custom subdomain, so no DNS records are needed).
- `index.html` loads the chat widget with one script tag pointing at `/widget.js` on that address.
- The backend only accepts requests from `https://surajkohli.com`.
- Why Northflank: it is free and always on. Free tiers that sleep (Render, Koyeb) would delay the chat button. Cloudflare Workers was ruled out because LangChain does not run there.
- More detail: `docs/BUILD_PLAN.md` in the career-chatbot repo.
