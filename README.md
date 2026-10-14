# testmira

A minimal dark blog built with [Astro](https://astro.build), inspired by Claude's clean aesthetic.

## Features

- 🌑 **Dark minimal design** — warm tones, clean typography
- 📝 **Markdown posts** — write in `.md` or `.mdx`
- 🧩 **HTML embed support** — drop raw HTML into your markdown
- ☁️ **Cloudflare Pages ready** — deploy in minutes
- ⚡ **Fast by default** — static site, zero JS by default

## Quick Start

```bash
npm install
npm run dev
```

Open [http://localhost:4321](http://localhost:4321).

## Writing Posts

Create `.md` files in `src/content/blog/`:

```markdown
---
title: "My Post"
description: "What this post is about"
pubDate: 2026-10-14
tags: ["astro", "blog"]
---

Your content here. HTML works too:

<div class="custom-card">
  <h3>Embedded HTML</h3>
  <p>This renders as real HTML!</p>
</div>
```

## Deploy to Cloudflare Pages

### Option 1: Via Cloudflare Dashboard
1. Push this repo to GitHub
2. Go to [Cloudflare Dashboard](https://dash.cloudflare.com) → Pages
3. Connect your GitHub repo
4. Build command: `npm run build`
5. Output directory: `dist`

### Option 2: Via CLI
```bash
npm run build
npm run pages:deploy
```

## Project Structure

```
├── src/
│   ├── content/
│   │   └── blog/          # Your .md posts live here
│   ├── layouts/           # Base + blog post layouts
│   ├── pages/             # Routes (index, blog, 404)
│   └── styles/            # Global CSS
├── public/                # Static assets
├── astro.config.mjs       # Astro config
└── wrangler.toml          # Cloudflare config
```

## License

MIT
