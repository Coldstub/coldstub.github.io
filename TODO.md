# TODO

## Last session

- 2026-11-26 — tokens synced to blog Style_Guide_v2; real hrefs for github / telegram / soundcloud (old `n3koraana` was 404) + [contact]; OG image; GhostBg layer; shell input (`help` / `ls` / `open` / `whoami` / `clear`). Resume: blog href, then deploy.

## Now (MVP)

- [ ] fill real hrefs: blog (still `#todo-blog` — blog not deployed yet)
- [x] fill real hrefs: github, telegram (t.me/ripwned), soundcloud (ripbny), contact (t.me/imwfso)
- [ ] deploy to GitHub Pages
- [ ] test: phone on 4G, every link opens (375px layout checked in emulation, no overflow)
- [x] test: JS disabled, links still visible

## Backlog — pick one per weekend, any order

- [x] OG image (1200×630) for Telegram / Discord link previews — `og.png`, source `og.html`
- [ ] custom domain (then update `og:url` / `og:image` in `index.html`)
- [x] background layer: inline SVG geometry, opacity ~0.06 (borrow blog GhostBg)
- [x] fake shell input: `help` / `ls` / `open <name>`
- [ ] Discord presence via Lanyard (needs Discord user ID)
- [ ] view counter via Cloudflare Workers + KV (only backend item)
