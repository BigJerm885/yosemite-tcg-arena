# Yosemite TCG — TCG-Arena files

Hosts the card images + game files for playing **Yosemite TCG** on [tcg-arena.fr](https://tcg-arena.fr).

- `images/` — 67 card faces + `cardback.png` + `banner.png`
- `CardList.json` — the 67-card list
- `Game_YosemiteTCG.json` — the game/board definition

## Publish (one time)

1. Create a free GitHub account (github.com) if you don't have one.
2. Make a new **public** repo named exactly **`yosemite-tcg-arena`** (no README — this folder already has one).
3. In Terminal, from this `repo/` folder, run the commands GitHub shows you for "push an existing repository", i.e.:
   ```
   git remote add origin https://github.com/YOURNAME/yosemite-tcg-arena.git
   git branch -M main
   git push -u origin main
   ```
4. Tell Claude your GitHub username — it will rebuild the two JSON files with your real URLs (or run `python3 ../build_tcg_arena.py YOURNAME`), then push again.
5. Your game link: on tcg-arena.fr/build, paste
   `https://raw.githubusercontent.com/YOURNAME/yosemite-tcg-arena/main/Game_YosemiteTCG.json`
   into box 4 and copy the generated link. Share it!

## Updating later

Edit anything, then `git add -A && git commit -m "update" && git push`.
