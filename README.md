# Aegis — Web Security Toolkit

A browser-based security assessment MVP built with HTML, CSS, and JavaScript.

## Run locally

```bash
python3 -m http.server 8000 --directory dist
```

Open http://localhost:8000. No package installation or build step is required.

## Features

- Weather-site demonstration, clearly labeled as fictional.
- Application-specific, template-based security test plans.
- Imported HTTP response analysis: CSP, HSTS, content type and frame protection, cookie flags, CORS, and selected secret patterns.
- Evidence, severity filters, curated remediation guidance, JSON exports, and local assessment history.
- Comparison of imported assessments for the same target.

## Current limits

This version does not crawl targets, perform active attacks, test authenticated permissions, or call an AI model. Explanations are curated; planning is template-based. Findings marked "Needs review" require verification. A passing check is not a guarantee of security.

Assessments are stored in browser localStorage. Raw imported responses are not persisted, and cookie values and matched secret values are omitted from findings. Remove sensitive information before importing. Only assess applications you are authorized to test.

External Google Fonts are optional; system fonts are used as fallback.

## Files

- `dist/index.html` — interface
- `dist/style.css` — responsive styles
- `dist/app.js` — workflow, history, plans, and exports
- `dist/engine.js` — deterministic response checks

## Planned integrations

Live AI explanations, verified target ownership, server-side scanning, and authenticated permission tests.
