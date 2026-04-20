# preview.thedrive.ai

Turn any URL into a preview image. PDFs, documents, slides, videos, code, and websites — just prepend the URL.

```
https://preview.thedrive.ai/{any-url}
```

No API key. No signup. No setup.

## Quick start

```html
<img src="https://preview.thedrive.ai/arxiv.org/pdf/1706.03762" />
```

That's it. You get a JPEG thumbnail of the first page.

## Live examples

| Type | URL | Preview |
|------|-----|---------|
| PDF | `arxiv.org/pdf/1706.03762` | ![](https://preview.thedrive.ai/arxiv.org/pdf/1706.03762?w=300&h=200) |
| Website | `github.com` | ![](https://preview.thedrive.ai/github.com?w=300&h=200) |
| PPTX | `dickinson.edu/.../sample.pptx` | ![](https://preview.thedrive.ai/www.dickinson.edu/download/downloads/id/1076/sample_powerpoint_slides.pptx?w=300&h=200) |
| Video | `w3schools.com/.../mov_bbb.mp4` | ![](https://preview.thedrive.ai/www.w3schools.com/tags/mov_bbb.mp4?w=300&h=200) |

## Usage

### HTML

```html
<a href="https://example.com/report.pdf">
  <img
    src="https://preview.thedrive.ai/example.com/report.pdf"
    alt="preview"
    width="600"
    height="400"
  />
</a>
```

### Next.js

```jsx
import Image from 'next/image'
import Link from 'next/link'

<Link href="https://example.com/report.pdf">
  <Image
    src="https://preview.thedrive.ai/example.com/report.pdf"
    alt="preview"
    width={600}
    height={400}
  />
</Link>
```

### Markdown

```markdown
![preview](https://preview.thedrive.ai/example.com/doc.pdf)
```

## Parameters

| Param | Default | Description |
|-------|---------|-------------|
| `w` | 600 | Width (50-2000) |
| `h` | 400 | Height (50-2000) |
| `q` | 95 | JPEG quality (1-100) |
| `nocache` | false | Skip cache for fresh render |

```
preview.thedrive.ai/example.com/doc.pdf?w=800&h=600&q=90
```

## Supported formats (67+)

| Category | Formats |
|----------|---------|
| Documents | PDF, DOCX, DOC, PPTX, PPT, XLSX, XLS, ODT, ODP, ODS, RTF, CSV |
| Images | JPG, PNG, GIF, WebP, SVG, AVIF, HEIC, HEIF, BMP, TIFF |
| Video | MP4, MOV, WebM, AVI, MKV, WMV, FLV, 3GP, M4V |
| Code | 30+ languages — Python, JavaScript, TypeScript, Go, Rust, Java, C/C++, and more |
| Markdown | MD, Markdown, Mdown |
| Text | TXT, LOG |
| Websites | Any URL — rendered via headless browser |

## Features

- **No API key required** — just use the URL
- **Social media cards** — auto OG tags for Discord, Slack, Twitter, LinkedIn
- **Caching** — 24h server cache + 7-day browser cache
- **Custom dimensions** — any size from 50px to 2000px
- **Fast** — response time in headers (`X-Response-Time`)

## Pricing

| | Free | Pro ($19/mo) |
|---|------|-------------|
| Rate limit | 30 req/min | 120 req/min |
| Formats | All 67+ | All 67+ |
| API key | Not needed | Included |
| Support | Community | Priority |
| SLA | — | 99.9% uptime |

[Get started](https://preview.thedrive.ai) | [API docs](https://preview.thedrive.ai/docs) | [Contact](mailto:contact@thedrive.ai)

## Use cases

- **File managers** — show document thumbnails
- **CMS / blog editors** — link preview cards
- **Search results** — visual thumbnails for indexed docs
- **Chat apps** — embed file previews
- **AI tools** — display retrieved documents visually
- **Emails** — inline document previews via `<img>` tags

## Links

- [Try it live](https://preview.thedrive.ai)
- [API documentation](https://preview.thedrive.ai/docs)
- [Blog](https://thedrive.ai/blog)

---

Built by [thedrive.ai](https://thedrive.ai)
