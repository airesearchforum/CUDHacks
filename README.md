# CUDHacks 2027: AI for the UAE

Website for CUDHacks 2027 ("AI for the UAE: Solving National Challenges"), hosted by the Software Engineering Club at Canadian University Dubai, supported by etisalat by e&. Fri 19 March 2027 (online) and Sat 20 March 2027 (on campus at CUD).

There are three tracks: Digital UAE, Sustainable UAE and Empowering UAE Communities. Each has suggested challenge statements, and teams can also propose their own UAE problem. The page also covers open data sources, impact-based judging and the 30-day follow-up demo and pilot path.

It's a static site: one `index.html` plus `assets/`. There's no build step.

## Before going live

Open `index.html` and fill in the `CONFIG` block near the bottom:

```js
const CONFIG = {
  registerUrl: "",   // your Google/Microsoft Form link
  contactEmail: "",  // organiser email
  kickoff: "2027-03-19T09:30:00+04:00"
};
```

Check the schedule times in the `#schedule` section as well. They are placeholders.

## Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "CUDHacks site"
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
