# Muse 1.2 Chat — Mobile & Desktop PWA

Single-file chat UI for `muse-spark-1.2` (`POST https://api.meta.ai/v1/responses`).

## Use
1. Open the deployed Vercel URL on phone or desktop.
2. Click ⚙︎ → paste `MODEL_API_KEY` → Save → Test connection.
3. Chat. History is saved in localStorage. Toggle Images / Web / GitHub at top.

## Deploy to Vercel (you — 1 command)
```bash
cd /Users/zackalexander/muse-chat
npx vercel --prod
# or: vercel --prod (if installed)
```
- Framework: Other / Static
- Output dir: `.` (just index.html + vercel.json)
- Vercel will give you https://your-project.vercel.app — share to phone, Add to Home Screen.

## Deploy to Lovable
1. Go to lovable.dev → New Project → Import → paste this `index.html` or GitHub repo.
2. Prompt: "Deploy this static PWA as-is, keep API calls client-side to api.meta.ai"
3. Publish — Lovable gives HTTPS URL.

## Local
```bash
cd /Users/zackalexander/muse-chat
python3 -m http.server 8000
# open http://localhost:8000
```
Do not open via file:// — CORS will block api.meta.ai.
