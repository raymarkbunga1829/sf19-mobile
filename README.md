# Stockfish 19 Mobile

Phone-first chess PWA that runs **Stockfish 19** (lite single-thread WASM) in a Web Worker.

Play vs the engine or use analysis mode. Works in iPhone/iPad Safari. Add to Home Screen for an app-like icon.

## One-click deploy on Vercel

1. Open: https://vercel.com/new/import?s=https://github.com/raymarkbunga1829/sf19-mobile
2. Import the repo (Framework Preset: **Other**; publish the repo root).
3. Deploy.
4. On iPhone: open the URL in Safari → Share → **Add to Home Screen**.

Repo: https://github.com/raymarkbunga1829/sf19-mobile

## Local

```bash
python3 -m http.server 8080
```

## Engine

- Worker: `engine/stockfish-19-lite-single.js` (Stockfish.js 19.0.0)
- WASM loaded from unpkg (`stockfish@19.0.0/bin/...`) so the repo stays small
- Rules: chess.js (BSD-2-Clause)

## License

Stockfish / stockfish.js are **GPL-3.0**. Keep this source public if you distribute the app.
