# student_assistant
AI chatbot for Students attending Puritan Reformed Theological Seminary. 

# PRTS Student Assistant

Student handbook chatbot for Puritan Reformed Theological Seminary. Built on Microsoft Copilot Studio + Web Chat.

## Deploy to GitHub Pages

1. Create a new repo on GitHub (or use an existing one).
2. Upload the contents of this folder to the repo root (or to a subfolder like `chat/`).
3. In the repo: **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: `main` → Folder: `/ (root)` → **Save**
4. Wait ~1 minute, then visit `https://<your-username>.github.io/<repo-name>/`.

## Allow your GitHub Pages origin in Copilot Studio

Once the page is live, the bot will refuse cross-origin requests until you allow the origin:

1. Open your bot in **Copilot Studio**
2. **Settings → Security → Web channel security** (or "Allowed domains")
3. Add your Pages URL, e.g. `https://<your-username>.github.io`
4. Save

## Files

- `index.html` — the chat page (GitHub Pages serves this at the repo root)
- `assets/prts-logo.png` — seminary logo used in the header and bot avatar

## If you rename the bot

The token endpoint URL in `index.html` (near the top of the `<script>` block, `tokenEndpoint = ...`) contains the bot's schema name. If you rename the bot in Copilot Studio, grab the new token endpoint from **Settings → Channels → Web app** and paste it in.
