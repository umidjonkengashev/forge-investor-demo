# FORGE — Steelworks Investor Preview

A mobile-first, installable Progressive Web App (PWA) for presenting an illustrative steel plant investment concept.

## Included
- Overview dashboard and project snapshot
- Interactive schematic plant explorer with selectable production zones
- Financial model with adjustable assumptions and live calculations
- Export current financial assumptions and outputs to a text file
- Project roadmap
- PWA manifest, icons, and service worker for offline use after first load
- Responsive layout for mobile, tablet, and desktop

## Important
All financial values, capacity, timeline, and project details are fictional demonstration assumptions. This is not an investment offer, feasibility study, valuation, or forecast. Replace all sample content with approved and independently validated project information before using it as a real investment presentation.

## Quick preview on a computer
You need Python 3 installed. In this folder run:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080` in your browser.

## Install on a phone
A PWA must be served from HTTPS (or localhost) to install and use offline features.

1. Upload the contents of this folder to a static host that provides HTTPS (for example, a static-site host).
2. Open the HTTPS URL on the phone.
3. Android / Chrome: use the browser menu or the app's install prompt and select **Install app** / **Add to Home screen**.
4. iPhone / Safari: tap **Share** → **Add to Home Screen**.
5. Open once while online; the service worker caches the app shell for subsequent offline use.

You do not need a backend for this prototype. Later, replace the demo assumptions in `app.js` with API responses and add authentication/database services once the business requirements are approved.

## Backend integration path
- Define real entities: projects, facilities, production lines, equipment, assumptions, scenarios, milestones, documents, users, and audit events.
- Validate formulas with a finance/engineering owner.
- Add an API layer and database (for example, PostgreSQL via a managed service) only after the data model and access rules are agreed.
- Separate public investor-facing data from confidential internal data; add role-based access and audit logs before using real project documents or financials.
