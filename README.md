# BillBuddy

A responsive bill and subscription tracker built as a Cloudflare Worker static site.

## Features
- Dashboard totals for this month, the next seven days, overdue bills, and recurring subscriptions
- Add, edit, delete, search, and filter bills
- One-time, weekly, biweekly, monthly, quarterly, and yearly recurrence
- Mark one-time bills paid; recurring bills advance to their next due date
- Spending breakdown by category
- Currency display settings
- JSON backup and restore
- Optional browser notifications
- Installable progressive web app with basic offline caching

## Data and privacy
BillBuddy v1 stores bill records in the browser's local storage on the current device. It does not send bill details to a server. Clearing browser data or changing devices can remove or leave behind data, so use **Settings → Export JSON** to keep a backup. Cloud sync and user accounts are not included in this first version.

## Run locally
```bash
npm install
npm run dev
```

## Deploy to Cloudflare Workers
1. Connect this repository to Cloudflare Workers.
2. Build command: leave blank (no build step).
3. Deploy command: `npm run deploy`.
4. Root directory: `/`.
5. Wrangler serves the `public` directory as static assets.

No API keys or paid services are required for the current version.
