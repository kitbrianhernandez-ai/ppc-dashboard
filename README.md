# Amazon PPC (Sponsored Products) Dashboard (demo)

A self-contained, single-file Sponsored Products management dashboard built with
Claude Code from live Amazon Ads data. **This is a de-identified demo** — every real
search term, campaign, keyword, ASIN and brand has been replaced with synthetic
values; the metrics and structure are preserved.

**Live page:** https://kitbrianhernandez-ai.github.io/ppc-dashboard/

## What it shows

- **Wasted spend & negatives** — search terms burning clicks/spend with no orders,
  surfaced as negative-keyword candidates.
- **Harvest** — converting search terms worth promoting into new exact/phrase targets.
- **Keyword & campaign tree** — spend, sales, ACOS and order rollups per ASIN.
- **Weekly review** — week-on-week campaign movement, flags and trend.
- **Best performers, competing terms, main words** — where the budget is working.

## How it's built

In production, Claude Code pulls live search-term and campaign data through an MCP
connector, computes the analysis, and rebuilds this HTML. Nothing is pushed back to
Amazon — negatives and new targets are delivered as review-ready files for human
sign-off.

_Single file — just open `index.html` in a browser._
