# Wolvbot GTM CRM — Bangalore ASRS VMI Pilot

A standalone single-file CRM dashboard for tracking outreach to Bangalore quick-commerce and VMI target accounts.

## How to use

Open `wolvbot_crm.html` directly in any browser — no server needed.

## Features

- **CRM view** — all 20 accounts with expand panels for Overview, Contact, Edit, and Notes
- **Contact tab** — fill in name, email, phone, LinkedIn, and next-step per account
- **Edit tab** — update category (dropdown), status, action, scores, demand, pitch, platforms
- **Notes tab** — timestamped follow-up notes per account
- **Summary page** — KPIs, pipeline funnel, top accounts, category/demand charts, activity feed
- **Add Account** — form with all fields including contact details
- **Export CSV** — downloads all data including contacts and notes

## Hosting on GitHub Pages

### First-time setup

1. Go to https://github.com/new
2. Name the repo `wolvbot-crm` (or anything you like)
3. Set it to **Public** (required for free GitHub Pages)
4. Click **Create repository**
5. Upload `wolvbot_crm.html` — rename it to `index.html` when uploading
6. Go to **Settings → Pages**
7. Under **Branch**, select `main` and folder `/root`, click **Save**
8. Your dashboard will be live at: `https://YOUR-USERNAME.github.io/wolvbot-crm/`

### Updating the file frequently

**Option A — Edit directly on GitHub (easiest)**
1. Go to your repo on github.com
2. Click `index.html`
3. Click the ✏️ pencil (Edit) icon
4. Make changes in the editor
5. Click **Commit changes** — live in ~30 seconds

**Option B — Use GitHub Desktop app**
1. Download from https://desktop.github.com
2. Clone your repo
3. Edit `index.html` locally in any text editor (VS Code recommended)
4. Click **Commit to main** → **Push origin**
5. Live in ~30 seconds

**Option C — Command line**
```bash
git clone https://github.com/YOUR-USERNAME/wolvbot-crm
cd wolvbot-crm
# edit index.html
git add index.html
git commit -m "update: added contact for HealthKart"
git push
```

## Data persistence note

All data lives inside the HTML file itself. When you update statuses, contacts, or notes in the browser, those changes exist only in that browser session. To make edits permanent, use **Export CSV** to save your data, then update the `accounts` array in the `<script>` section of `index.html` and re-upload.

For a persistent version that saves across sessions, consider adding a Google Sheet backend via Google Apps Script (ask for instructions).

## File structure

```
wolvbot-crm/
└── index.html    ← the entire CRM (rename from wolvbot_crm.html)
└── README.md     ← this file (optional)
```
