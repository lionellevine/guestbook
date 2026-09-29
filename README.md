# Lionel Levine's Guestbook

Published at https://lionellevine.github.io/guestbook/ (GitHub Pages, from this repo's root).

This repo is written to by a GitHub Action in the private moderation inbox: it appends
approved entries to `entries.json`, renders `*.template.html` to the matching pages, and
writes `investigation.json`. Edit the templates here; the next approval (or a manual run
of the inbox's "moderate" workflow) re-renders the pages.

Files:
- `entries.json`: every published entry (visitor text is never rewritten).
- `challenges.json`: the research challenges (slug, question, page, bins, moves). A
  template declares its challenge with `<!-- challenge: slug -->`.
- `adjudications.json`: Lionel's read of ledger rows, inferred from his published
  replies (verdict, note, the reply entry ids it rests on), argument groups, and the
  classification of older verifies. Maintained by Claude on Lionel's behalf; Lionel
  approves the note wording. Update it, push, re-render.
- `*.template.html`: the pages, with placeholders filled by the inbox's `publish.py`.
