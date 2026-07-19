# Hawk Talk Solutions Ltd - Launch checklist and SEO Reference

This document lists the placeholders that need to be replaced with real client values prior to deploying the website to production.

## Actionable Placeholders

| Placeholder | Purpose | Location in Code |
|---|---|---|
| `[EMAIL_ADDRESS]` | Legal contact email for GDPR and contact details | Footer across all pages, contact form labels, profiles on about and contact pages |
| `[LANDLINE_NUMBER]` | Primary phone number for business contact | Header/Footer references, contact page layout details |
| `[COMPANY_NUMBER]` | Companies House number for Hawk Talk Solutions Ltd | Page footer fine print |
| `[FORM_ENDPOINT_PLACEHOLDER]` | The backend form handling service endpoint (e.g., Formspree, Web3Forms, etc.) | `<form>` action attributes on `index.html` and `contact.html` |

## Verification & Deployment Guidelines

1. **Placeholder Search**: Use a search tool (like grep or VSCode search) to query for `CLIENT TO CONFIRM` to locate every instance of the above placeholders.
2. **Relative Links**: Ensure that the project is built using only relative paths (`services/...` and `../...`) so it loads properly if hosted under a GitHub Pages subpath (e.g., `https://username.github.io/hawk_talk_multipage/`).
3. **Form Parameter Validation**: The form dropdown pre-selection works automatically on page load of `contact.html` when loaded via `contact.html?service=[service-slug]`. Ensure CTAs on all service detail pages link correctly to `../contact.html?service=[service-slug]`.
