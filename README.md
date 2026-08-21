# Developer Depth vs Framework-Only

This project captures the theme of **full-stack understanding** versus **framework-only knowledge** in modern web development (especially React).

## The Core Imagery

![Developer Knowledge Levels](assets/developer-knowledge-levels.jpg)

The visual contrasts two types of developers debugging the same apparent issue:

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

## Project Goals

- Provide a clear, shareable visual for talks and team culture
- Encourage deeper platform knowledge alongside framework skills
- Serve as a starting point for more educational content around web fundamentals

## License

Feel free to use the imagery and text for educational purposes, blog posts, conference talks, and internal training.

---

Built with ❤️ for developers who want to understand *why* things work, not just *how* to make the framework happy.
