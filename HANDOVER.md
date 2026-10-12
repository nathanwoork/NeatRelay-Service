# NeatRelay Service — handover

## Current state

Date: 6 October 2026. Customer-facing prototype published; live site and successful GitHub Pages deployment verified.

Repository: https://github.com/nathanwoork/NeatRelay-Service

Website target: https://nathanwoork.github.io/NeatRelay-Service/

## Change log

### 6 October 2026 — first customer-service design

- Created a separate public repository as requested by Nathan.
- Built seven content routes and responsive ink/teal/mint visual design.
- Added service pricing/scope, interactive package chooser, process walkthrough, founder profile, planned specialist roles, company concept/vision and contact.
- Built a fictional project-room flow with brief, board and gated acceptance checklist.
- Public contact address confirmed by Nathan: nathan.woork@gmail.com. Enquiries become a visible mailto draft; nothing is sent automatically or stored by a server.
- No customer, registration, staffing, booking, payment or savings claims invented.
- JavaScript syntax passed. Browser and deployment checks are being completed before release.

## Next decisions

Confirm working brand and real business details; validate packages; review final public copy; decide whether a secure enquiry backend and client portal are warranted. Keep client records out of this public repository. The operations dashboard is a separate project at https://github.com/nathanwoork/NeatRelay.

Every change must append a dated progress entry here with verification and unresolved issues; see AGENTS.md.

### 6 October 2026 — local release checks passed

Dashboard: syntax and meaningful backup validation passed, including legacy imports, assignment round-trip, invalid roles/stages/dates and safe escaping. Browser checks confirmed handoff saving, reload persistence, brief content and backup inclusion; synthetic QA data was reset. Mobile delegation layout has no horizontal overflow at the tested 390px viewport.

Service: desktop and mobile layout/navigation checked; package recommendation and contact package selection passed; email draft points to the confirmed address without sending; fictional acceptance is gated by all four checklist items. Process, People and About views checked; no service console errors observed. No horizontal overflow in tested mobile views.

Both public repositories exist and GitHub Pages is configured for main/root. Publishing and public deployment verification follow this entry. Remaining limitations: static prototypes, local-only delegation, no real client portal or enquiry backend, draft pricing and unvalidated business assumptions.

### 6 October 2026 — published and verified

- Dashboard source: https://github.com/nathanwoork/NeatRelay — application commit 174189f7206ff2cdafe0f839c8d9d1fbc1cb81b7.
- Dashboard site: https://nathanwoork.github.io/NeatRelay/ — live delegation page verified; fresh handoff register contains no QA assignments.
- Service source: https://github.com/nathanwoork/NeatRelay-Service — application commit ac00ae219298fe7c833915ed7f9c3b5dce2c197f.
- Service site: https://nathanwoork.github.io/NeatRelay-Service/ — live home and pricing navigation verified.
- Both application commits have successful GitHub Pages workflow results. Desktop screenshots saved in local focused/verification; mobile checks and interactions are recorded above.
- Portfolio repository commit 81b5d335503a6d1382d3267bcacd63f7ca9a95ea publishes a redirect only at the legacy neatrelay/index.html plus legacy documentation. The root portfolio is preserved. Redirect deployment verification is recorded in the central local log.
- This release also updates the workspace index and handover instructions. Historical entries above describe earlier states; this entry and Current state take precedence.

Next: Nathan reviews the service copy and draft prices, prepares one complete synthetic workflow with failure tests, and validates the offer before accepting client work. Future hires can be planned through Delegate work; actual shared assignments remain in Trello or another agreed system. No invitations, hiring, emails, payments or client-data processing occurred in this release.

### 12 October 2026 — Relay Spectrum redesign in progress

Applied Nathan’s dashboard references and researched Asana/monday examples. Added shared semantic colour tokens, locally hosted licensed Manrope/Space Grotesk fonts, an honest task-completion dial, themed dashboard/service views and a reusable visual design guide. Storage, backup schema, pricing and service boundaries are preserved. Desktop first pass inspected; responsive/interaction verification and publishing follow.

### 12 October 2026 — redesign verification complete; publishing

Relay Spectrum now covers both sites, including boards, forms, delegation, pricing, profile/vision and the client demo. The canonical shared kit is in focused/design-system; each repository includes DESIGN-LANGUAGE.md, design-system.html, colour tokens, embedded fonts and OFL notices. Local playbook, brand memo and workspace index now point to this direction.

Verification: desktop (approximately 1280px), tablet (820px), phone (390px) and narrow phone (320px) were rendered. All dashboard/service routes were checked for phone overflow; dashboard secondary routes also checked at desktop. Tablet sidebar overlap was found and fixed by aligning CSS and JavaScript drawer breakpoints at 900px; menu navigation, Enter and Escape were rechecked. Task filtering, edit dialog, count recalculation (4/24 to 5/24), reload persistence and restoration to the original task status passed. Legacy backup/delegation tests passed. Service package selection, email draft preparation without sending, demo workboard and four-check acceptance gate passed. The design specimen status/density controls passed. No JavaScript errors appeared in inspected tabs.

Selected text colour pairs meet 4.5:1 (6.0–13.8:1 in checked semantic pairs). Shared files are byte-identical across the two sites. No full accessibility certification or cross-browser/device-lab testing is claimed. Fonts cover the current Latin content; non-Latin localisations require a deliberate font extension. The dashboard is still browser-local with no automatic Trello sync; service remains a prototype. No new customer, hiring or financial outcomes are implied.

Next: publish and verify GitHub Pages, then Nathan can review the visual direction. Continue business validation and implementation tasks separately.
