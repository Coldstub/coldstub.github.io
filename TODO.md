# TODO

## Last session

- 2026-11-26 — tokens synced to blog Style_Guide_v2; real hrefs for github / telegram / soundcloud (old `n3koraana` was 404) + [contact]; OG image; GhostBg layer; shell input (`help` / `ls` / `open` / `whoami` / `clear`). Deployed to https://coldstub.github.io/. Then: dropped [blog] placeholder (shortcuts 1–4), kana name + `:lang(ja)` font, tagline "reverse engineer · security researcher", animation types only the first `whoami` (once per session; links visible ~0.4s), background geometry moved right of the text column (≥1100px only), OG image re-rendered. Resume: blog link.
- 2026-11-27 — ported 0002-matrix-balanced.patch by hand (its base commit — pure-Matrix palette + `art.webp` — never landed here): Matrix Balanced tokens; IBM Plex Mono self-hosted; name = kana + romaji only; [discord] added as 4, [contact] → 5; background lines kept, recolored green (no `art.webp` yet); OG image re-rendered. Resume: blog link; art.webp if wanted.

## Now (MVP)

- [ ] add [blog] back once the blog is live (removed rather than left as a dead `#` link), then renumber the 1–N shortcuts and the hint text
- [x] fill real hrefs: github, telegram (t.me/ripwned), soundcloud (ripbny), contact (t.me/imwfso)
- [x] deploy to GitHub Pages — live at https://coldstub.github.io/
- [ ] test: phone on 4G, every link opens (375px layout checked in emulation, no overflow)
- [x] test: JS disabled, links still visible

## Backlog — pick one per weekend, any order

- [x] OG image (1200×630) for Telegram / Discord link previews — `og.png`, source `og.html`
- [ ] custom domain (then update `og:url` / `og:image` in `index.html`)
- [x] background layer: inline SVG geometry, opacity ~0.06 (borrow blog GhostBg)
- [x] fake shell input: `help` / `ls` / `open <name>`
- [ ] Discord presence via Lanyard (user ID 1574971631200243784; account must join the Lanyard server)
- [ ] view counter via Cloudflare Workers + KV (only backend item)
