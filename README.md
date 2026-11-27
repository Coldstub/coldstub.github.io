# coldstub links

Single-file link page. No build step, no dependencies.

## Edit

- links: `index.html` → `<ul class="links">`
- colors / spacing: `index.html` → `:root` (mirrors Coldstub-Blog `Style_Guide_v2`)
- shell commands: `index.html` → `commands` in the script
- OG image: edit `og.html`, then re-render `og.png`:

```powershell
& "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --headless=new --hide-scrollbars --force-device-scale-factor=1 --window-size=1200,630 --screenshot="$PWD\og.png" "file:///$($PWD -replace '\\','/')/og.html"
```

## Local preview

```sh
python3 -m http.server 8000   # open http://localhost:8000
```

## Deploy (GitHub Pages, user site)

```sh
git init && git add -A && git commit -m "init"
gh repo create coldstub.github.io --public --source=. --push
# repo named <user>.github.io serves main/root at https://<user>.github.io
```

## Rules

- `main` is always deployable; unfinished work stays on a branch.
- One TODO item per session; update `TODO.md` before stopping.
- No docs beyond README + TODO. Git log is the changelog.
