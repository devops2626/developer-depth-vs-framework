# Developer Depth vs Framework-Only

This project captures the theme of **full-stack understanding** versus **framework-only knowledge** in modern web development (especially React).

**Live page:** Enable GitHub Pages on the `main` branch (Settings → Pages → Source: Deploy from a branch → main / root) then visit  
`https://devops2626.github.io/developer-depth-vs-framework/`

## The Core Imagery Theme

The original visual (shared in the conversation that started this repo) contrasts two types of developers debugging the same apparent issue:

### 👨‍💻 Framework-Only Developer
- Checks only if the right React hook is used
- Looks at the code surface

### 🛠️ Deep / Platform-Aware Developer
- Inspects HTTP request headers to see if caching is enabled
- Verifies whether the API is returning fresh data
- Checks if the frontend is caching the response
- Looks at browser cache
- Reviews API response headers
- Confirms frontend data is stored correctly

## Why This Matters

Modern frameworks (React, Next.js, etc.) abstract a lot of complexity. That is powerful — until something goes wrong in the layers underneath:

- HTTP caching (Cache-Control, ETag, etc.)
- CDN / edge caching
- Browser HTTP cache
- Service workers / local storage / IndexedDB
- API freshness guarantees
- Stale-while-revalidate strategies

A developer who only knows the framework will keep changing hooks and state management. A developer who understands the full request lifecycle will look at the network tab first.

## What's in this repo

- `index.html` — Educational page featuring:
  - Side-by-side comparison of framework-only vs platform-aware thinking
  - **Interactive debugging checklist** with:
    - Clickable checkboxes
    - Live progress bar + counter
    - localStorage persistence (progress survives page reloads)
    - Reset button
    - Completion celebration banner
  - **Dark / Light mode toggle** (top-right)
    - Preference saved in localStorage
    - Falls back to system preference on first visit
  - **Visitor chat** powered by [Giscus](https://giscus.app) (GitHub Discussions)
- This README

## Enable visitor chat (Giscus) — one-time setup

1. Go to the repo **Settings → General → Features** and enable **Discussions**.
2. Visit [https://giscus.app](https://giscus.app).
3. Select repository: `devops2626/developer-depth-vs-framework`.
4. Choose a Discussions category (e.g. **General**).
5. Copy the generated `data-repo-id` and `data-category-id`.
6. Paste them into the Giscus `<script>` tags in `index.html` (replace the empty values).
7. Install the **Giscus** GitHub App when prompted.

After that, visitors can sign in with GitHub and chat on the page.

## Project Goals

- Provide a clear, shareable visual + page for talks and team culture
- Encourage deeper platform knowledge alongside framework skills
- Serve as a starting point for more educational content around web fundamentals

## How to use

1. Star / fork if useful
2. Enable GitHub Pages (see above) to host the landing page
3. Use the interactive checklist during real debugging sessions or onboarding
4. Toggle dark/light mode with the button in the header
5. Enable Giscus (steps above) so visitors can chat
6. Drop the original imagery into `assets/` if you want to host it yourself

## License

Feel free to use the text, checklist, and theme for educational purposes, blog posts, conference talks, and internal training.

---

Built with ❤️ for developers who want to understand *why* things work, not just *how* to make the framework happy.
