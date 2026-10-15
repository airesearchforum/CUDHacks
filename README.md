# CUD Agent Hackathon 2026

Website for the CUD Agent Hackathon, hosted by the Software Engineering Club at Canadian University Dubai in partnership with etisalat by e&. Fri 20 to Sat 21 November 2026.

It's a static site: one `index.html` plus `assets/`. There's no build step.

## Before going live

Open `index.html` and fill in the `CONFIG` block near the bottom:

```js
const CONFIG = {
  registerUrl: "",   // your Google/Microsoft Form link
  contactEmail: "",  // organiser email
  kickoff: "2026-11-20T09:30:00+04:00"
};
```

Check the schedule times in the `#schedule` section as well. They are placeholders.

## Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "CUD Agent Hackathon site"
git branch -M main
git remote add origin https://github.com/<you>/cud-agent-hackathon.git
git push -u origin main
```

Then go to **Settings → Pages → Source: Deploy from a branch → `main` / `(root)`**.
The site will be live at `https://<you>.github.io/cud-agent-hackathon/`.

## Preview locally

```bash
python -m http.server 8000
```
