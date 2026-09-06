# Lionel Levine's Guestbook

Published at https://lionellevine.github.io/guestbook/ (GitHub Pages, from this repo's root).

This repo is written to by a GitHub Action in the private moderation inbox: it appends
approved entries to `entries.json`, renders `*.template.html` to the matching pages, and
writes `investigation.json`. Edit the templates here; the next approval (or a manual run
of the inbox's "moderate" workflow) re-renders the pages.
