# Knowledge Garden — Workspace Context

**What this is:** GreenSeek's single source of truth. Every fact used in marketing
content must trace back to a doc in this garden.

**Structure**
- `product/` — what GreenSeek is and does (features, plans, pricing, privacy)
- `brand/` — how we talk about it (voice, pillars, audiences)
- `faq/` — customer-facing answers, mirrored from the public knowledge base
- `glossary/` — generated definition pages for AI search (GEO). Don't hand-edit; regenerate.
- `_inbox/` — raw uploads. Curate into proper docs, then delete from inbox.
- `_index/` — generated. Never edit by hand.

**How to answer a question from the garden**
1. Search `_index/index.json` for keyword matches (or run `tools/ask_garden.py --q "..."`).
2. Open only the top 2–3 docs.
3. Answer with citations: `(source: product/pricing-plans.md)`.
4. If the garden doesn't contain the answer, say so — do not guess.

**Curation standard:** one topic per file, first line is an H1 title, first paragraph
is a self-contained summary (the index uses it), facts as bullet lists, no fluff.
