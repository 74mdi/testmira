---
title: "Writing in Markdown"
description: "A quick guide on how to write posts for this blog."
pubDate: 2026-10-14
tags: ["guide", "markdown"]
---

Every post is a `.md` file in `src/content/blog/`. Here's what you need to know.

## Frontmatter

Every post starts with YAML frontmatter:

```markdown
---
title: "Your Post Title"
description: "A short description"
pubDate: 2026-10-14
tags: ["tag1", "tag2"]
---
```

## Supported fields

| Field | Required | Description |
|-------|----------|-------------|
| `title` | Yes | Post title |
| `description` | No | Short summary |
| `pubDate` | Yes | Publication date |
| `updatedDate` | No | Last update date |
| `tags` | No | Array of tags |
| `draft` | No | Set `true` to hide from listings |
| `heroImage` | No | Path to hero image |

## Markdown features

Everything standard works: **bold**, *italic*, `inline code`, links, images, lists, blockquotes, tables, and code blocks with syntax highlighting.

## HTML embedding

You can drop raw HTML anywhere in your markdown:

<blockquote style="border-left: 3px solid #d4a574; padding-left: 1rem; color: #a8a29e; font-style: italic;">
  This is a custom blockquote using HTML.
</blockquote>

That's it. Write, push, done.
