---
name: convert-to-md
description: >
  Fetch any public webpage as clean, readable Markdown using the convert-to.md service.
  Strips all HTML noise (scripts, styles, nav, ads) so only the actual content remains —
  dramatically reducing token usage compared to raw HTML. Use when you need to read,
  analyze, or extract content from a URL as Markdown.
argument-hint: "[url]"
user-invocable: true
---

# convert-to-md

Convert any public webpage to clean, readable Markdown — using far fewer tokens than raw HTML.

## Why use this over raw HTML or WebFetch?

Raw HTML is full of scripts, styles, navigation, ads, and boilerplate that waste tokens. convert-to-md strips all of that and returns only the actual content as clean Markdown, typically **reducing token usage by 50-90%** compared to fetching raw HTML. Use `mode=article` to strip even further down to just the main content.

## When to use this skill

Use this skill when you need to:

- **Reduce token usage** — fetch web content as clean Markdown instead of bloated HTML
- Read or analyze the content of a web page
- Extract article text, documentation, or blog content from a URL
- Get a clean Markdown version of a page for summarization or comparison
- Fetch web content that WebFetch might struggle with (large pages, complex HTML)

## How to use

### Option 1: API (fastest, no install needed)

Fetch `https://convert-to.md/<url>` using WebFetch or curl:

```
https://convert-to.md/example.com
https://convert-to.md/https://en.wikipedia.org/wiki/Markdown
```

The URL can be bare (`example.com`) or full (`https://example.com`).

### Option 2: CLI

```bash
npx convert-to-md <url>
```

Or if installed globally (`npm i -g convert-to-md` / `brew install convert-to-md/tap/convert-to-md`):

```bash
convert-to-md <url>
```

## Query parameters (API)

| Parameter | Effect |
|-----------|--------|
| `raw=true` | Return Markdown only, without YAML front matter |
| `refresh=true` | Bypass cache, force a fresh fetch |
| `mode=article` | Extract only the main article content (uses Mozilla Readability) |

Combine them: `https://convert-to.md/example.com?raw=true&mode=article`

## CLI flags

| Flag | Description |
|------|-------------|
| `--raw` | No YAML front matter |
| `--refresh` | Bypass cache |
| `--output <file>` | Write to file instead of stdout |
| `--timeout <duration>` | HTTP timeout (default: `20s`) |

## Response format

By default, responses include YAML front matter with metadata:

```yaml
---
title: Page Title
source: https://example.com/article
author: John Doe
site: Example Site
published: 2024-03-04T12:00:00Z
lang: en
converted: 2024-03-04T12:34:56.789Z
---

# Article content as Markdown...
```

Use `raw=true` to get just the Markdown content without the front matter.

## Response headers (API)

| Header | Value |
|--------|-------|
| `X-Source-URL` | Final resolved URL (after redirects) |
| `X-Cache-Status` | `HIT` or `MISS` |
| `X-Extraction-Method` | `full`, `readability`, or `readability-fallback` |

## Extraction modes

- **`full`** (default) — Entire page body, stripped of scripts/styles/hidden elements. Best for LLM consumption.
- **`article`** (`mode=article`) — Main article only via Mozilla Readability. Falls back to cleaned full extraction if Readability drops too much content.

## Limits

- **Rate limit**: 30 requests/minute per IP
- **Max page size**: 10 MB
- **Fetch timeout**: 10 seconds
- **Cache TTL**: 1 hour (use `refresh=true` to bypass)
- **Protocols**: HTTP and HTTPS only

## Examples

Fetch a Wikipedia article:
```bash
curl "https://convert-to.md/en.wikipedia.org/wiki/Markdown?mode=article&raw=true"
```

Fetch documentation with metadata:
```bash
npx convert-to-md https://docs.github.com/en/get-started
```

Save to file:
```bash
npx convert-to-md --output article.md --raw https://example.com/blog/post
```
