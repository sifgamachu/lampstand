# Lampstand *(working title)*

**Your calling, posted daily.** Marketing site + calling quiz for Lampstand — the content tool from the ministry behind [Deep Bible Stories](https://deepbiblestories.com/), watched by 80 million on YouTube.

## What's here
| File | Purpose |
|---|---|
| `index.html` | Landing page — live AI script demo, waitlist |
| `quiz.html` | "Which voice in Scripture shares your calling?" — 8 patterns, client-side scoring |
| `privacy.html` | Plain-language privacy policy (religious-data handling) |
| `404.html` | "This lamp isn't lit yet" |
| `og-image.jpg` | Social share card (1200×630) |
| `vercel.json` | Clean URLs + cache headers |

## Stack
Zero-build static HTML. Waitlist → Supabase (`lampstand_waitlist`, insert-only RLS). Script demo → `lampstand-generate` edge function (Claude) with graceful local fallback.

## Deploy
Import this repo at [vercel.com/new](https://vercel.com/new) — no framework, no build command, output dir `.`
