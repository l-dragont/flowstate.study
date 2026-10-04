# Scam Squad

A satirical, browser-based call-center game (inspired by the idea of co-op "scam call center" games). Fictional victims, no real scam scripts; each call ends with a scam-awareness lesson.

## Run locally
Open `index.html` in a browser (no build step).

## Put it on GitHub
```bash
git init && git add . && git commit -m "Scam Squad"
git branch -M main
git remote add origin https://github.com/YOUR_USER/scam-squad.git
git push -u origin main
```

## Deploy to Vercel
1. vercel.com → **Add New → Project** → import the repo.
2. Framework preset: **Other**. No build command, no output directory.
3. Deploy. Every push to `main` redeploys.

## Multiplayer note
Vercel can't host WebSocket servers. For real online co-op, add a hosted realtime service (Supabase Realtime, Ably, PartyKit) and sync the `S` state object.
