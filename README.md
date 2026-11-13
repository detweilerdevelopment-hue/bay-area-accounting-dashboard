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
