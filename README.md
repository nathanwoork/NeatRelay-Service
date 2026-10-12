# NeatRelay Service

Customer-facing design prototype for a founder-led Malaysian workflow consulting service.

- Website: https://nathanwoork.github.io/NeatRelay-Service/
- Repository: https://github.com/nathanwoork/NeatRelay-Service
- Operations dashboard: https://nathanwoork.github.io/NeatRelay/
- Current progress and next steps: [HANDOVER.md](HANDOVER.md)

## Experience

Seven routes: Home, Services, How it works, Client demo, People, About and Contact. The ink/teal/mint/off-white palette and handoff motif match the operations dashboard.

- Service chooser and expandable package exclusions.
- Four-stage service walkthrough.
- Fictional client room: intake brief → work board → acceptance checklist. Interactions are in memory and clear on reload.
- Enquiry form prepares a visible email draft to Nathan's confirmed public address. The visitor reviews it and opens their own email app to send. There is no form backend, automatic send, booking, payment or CRM integration.
- Nathan is the only named founder. Other specialist roles are explicitly planned, not current staff or partnerships.

The RM650 / RM1,800 / RM450 prices are draft pilot hypotheses. Company registration/name checks, availability, real delivery capability and demand remain unverified. Do not add fabricated testimonials or results.

## Development and release

Static HTML/CSS/JavaScript, no dependencies or build step. Serve the folder with a local static server. GitHub Pages publishes `main` from `/ (root)`; `.nojekyll` disables Jekyll processing.

Update HANDOVER.md whenever changing code, content, design or deployment. Preserve dated history and record tests, unresolved issues and next steps. Do not publish personal prospect records, private finances, credentials, or local dashboard exports.

Before making the service operational: validate the offer, confirm legal/business arrangements, review accessibility and real content, define privacy/retention and support, and design a secure enquiry/client-portal backend if needed. The visible demo is not authentication or a production customer system.

## Relay Spectrum redesign · 12 October 2026

The current visual language is Relay Spectrum. See [the visual guide](design-system.html) and [design documentation](DESIGN-LANGUAGE.md). Shared assets: relay-tokens.css, fonts.css and FONT-LICENSES.txt; relay-theme.css contains this site’s application. Fonts are locally embedded under SIL OFL. Existing behaviour and storage remain unchanged.
