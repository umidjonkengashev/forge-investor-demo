# FORGE — Steelworks Investor Preview v1.1

A polished, multilingual, mobile-first investor demo for a conceptual steelworks project. Static frontend only; no backend, credentials, analytics, or external API are required.

## Included
- Russian, English, and Uzbek interface with remembered language preference.
- Project overview, interactive plant-zone explorer, editable financial scenario model, and roadmap.
- Base, upside, and stress-test scenarios.
- Financial outputs recalculate immediately when assumptions change.
- Export current assumptions and outputs to CSV (Excel / Google Sheets compatible).
- Model assumptions persist locally in the browser on that device.
- Installable PWA manifest, app icons, service-worker offline cache, responsive mobile layout.
- Vercel-ready static hosting configuration.

## Run locally
Open the folder in a terminal and run:

```bash
python -m http.server 8080
```

Then visit `http://localhost:8080`.

## Deploy to Vercel
1. Upload the contents of this folder to a GitHub repository.
2. Import the repository in Vercel.
3. For this static HTML app, leave the build command empty and set the output directory to `.` (the project root).
4. Deploy. HTTPS is required for PWA installation and service-worker features.

## Install on a phone
- Android: open the HTTPS site in Chrome and choose **Install app** / **Add to Home screen**.
- iPhone: open the HTTPS site in Safari, tap **Share**, then **Add to Home Screen**.

## Important disclaimer
All plant details, dates, capacities, prices, costs, and financial results are illustrative placeholders for interface demonstration only. They are not verified project information, an investment offer, or a financial forecast. Validate the real technology, market assumptions, CAPEX/OPEX, permitting, and schedule before using the demo in an investor decision.

## Technical notes
- Plain HTML, CSS, and JavaScript; no build step or package installation required.
- No database or server-side processing. Browser-local preferences are stored only on the current device.
- External Google Fonts may not load offline; system font fallbacks are included.


## Investor-first dashboard refresh
The overview now prioritizes investor decision metrics: CAPEX, modeled annual revenue, EBITDA, EBITDA margin, simple payback, break-even utilization, cost structure, scenario comparison, and due-diligence questions. The figures are illustrative placeholders and must be replaced with verified project inputs.
