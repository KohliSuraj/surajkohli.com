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
- **PostHog** (US cloud), loaded by a snippet in the `<head>` of `index.html`. It records page views with referrer, UTM tags, location and device, and sets a cookie so repeat visitors are recognized.
- The chat widget sends its own events to PostHog: `chat_opened`, `question_asked`, `chat_error`, `citation_opened`, `linkedin_clicked`. Each carries `conversation_id`, the same ID the backend uses for the LangSmith thread, so a PostHog visitor can be matched to their conversation in LangSmith.
- Cloudflare stays for now as a second count: ad blockers block PostHog but rarely Cloudflare's beacon.
- In the PostHog project settings, turn on "Discard client IP data" so only the derived country and city are stored.

## Chatbot

- The backend lives in a separate repo, `KohliSuraj/career-chatbot`.
- Hosted on the **Northflank** free sandbox as one always-on container.
- Address: `https://p01--career-chatbot-backend--zmby9qq4v8rg.code.run` (no custom subdomain, so no DNS records are needed).
- `index.html` loads the chat widget with one script tag pointing at `/widget.js` on that address.
- The backend only accepts requests from `https://surajkohli.com`.
- Why Northflank: it is free and always on. Free tiers that sleep (Render, Koyeb) would delay the chat button. Cloudflare Workers was ruled out because LangChain does not run there.
- More detail: `docs/BUILD_PLAN.md` in the career-chatbot repo.
