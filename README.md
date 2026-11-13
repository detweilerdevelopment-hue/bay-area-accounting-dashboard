# Bay Area Accounting Dashboard

A minimal, responsive dashboard for reviewing 20 researched accounting and tax professional contacts across area codes 408, 415, 925, 831 and 650.

## Run locally

Open `dist/index.html` in a browser, or serve the static directory:

```sh
python3 -m http.server 8000 --directory dist
```

Then visit http://localhost:8000. No build step or dependencies are required.

## Features

- Search by name, firm, email or city
- Filter by area code and professional role
- Inspect source links and qualification notes
- Select a 10-contact sample or a custom selection
- Export selected or filtered records as CSV
- Retain selection in browser local storage

## Files

- `dist/index.html`: layout and styling
- `dist/app.js`: filters, selection, details and CSV export
- `dist/data.js`: 20 sourced research candidates and evidence links
- `.openai/hosting.json`: existing ChatGPT Sites deployment configuration

## Data qualification

Research date: November 13, 2026. These are research candidates, not an accepted or fully verified marketing list. Email deliverability, named mailbox ownership and firm headcount under 10 remain unconfirmed. Record-specific exceptions are documented in the dashboard and CSV exports. Publicly listed contact details may change.

## Validation

JavaScript syntax checks and dataset checks passed: 20 records, 20 unique emails and the five requested area codes. Visual browser QA was unavailable in the build environment.

## Contact dataset upload pending

The `dist/data.js` file contains an empty placeholder; the researched contact dataset has not been uploaded. Publishing the researched personal contact details to this public repository requires explicit approval. The dashboard loads with an explicit empty state until the researched dataset is approved for public release.

## Deploy on Vercel

Import the repository with **Root Directory** set to the repository root (leave it blank), and use the **Other** framework preset. The committed `vercel.json` serves `dist/` directly with no install or build command. Deploy the latest `main` commit. No database, environment variables, or API keys are required.

A successful deployment with a root-page 404 usually means Vercel served the repository root instead of `dist/`. This configuration explicitly sets the output directory. If an older deployment is still selected, deploy the latest commit from `main`.
