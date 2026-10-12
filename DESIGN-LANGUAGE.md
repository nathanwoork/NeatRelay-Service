# Relay Spectrum · design language 1.0

Created for Nathan and NeatRelay, 12 October 2026. A reusable foundation, not a requirement that every future brand look identical.

## Visual thesis

**Clear work, with a little energy.** A founder should be able to see the next action without studying an intimidating control room. A quiet warm canvas holds purposeful blocks of colour; dark rounded typography anchors the page. Connected handoff shapes express NeatRelay's actual work: a decision becoming an owned next step.

The dashboard emphasises density, task state and honest progress. The service site uses the same foundation at an editorial scale, with a diagram of the service instead of unrelated lifestyle photography. The N mark keeps its existing path; a yellow asymmetric container gives it a more recognisable signature.

## Research and reference decisions

Nathan's seven supplied references: Sundays contributes generous task rows and pale colour families; Panze contributes compact project summaries; ShipNow contributes consistent category/status emphasis; Ofspace contributes warm mixed-colour metric panels; the dark board contributes readable column grouping; Shikra contributes compartmentalised hierarchy; the yellow dashboard contributes a focal progress indicator. These are composition references, not assets to copy. No third-party screenshot, avatar, logo or fictional financial data is shipped.

Additional research, reviewed 12 October 2026:
- [Asana: colour coding projects and tags](https://asana.com/inside-asana/colored-projects-and-tags) — colour works as a chosen organisational cue on a restrained base. This is an older design rationale, not a claim about current Asana features.
- [monday: overview widget](https://support.monday.com/hc/en-us/articles/360007078739-The-Overview-Widget) — overview summaries should lead to understandable project details.
- [monday: dashboards](https://monday.com/w/dashboards) — study the relationship between numbers, charts and actionable work. NeatRelay's dial uses only actual saved task counts; no invented activity or revenue chart.
- [Manrope](https://fonts.google.com/specimen/Manrope) and [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) — selected for legible UI text and distinctive open, geometric headings.

## Palette and meaning

| Role | Value | Use |
|---|---|---|
| Ink | #202725 | Text and primary actions |
| Canvas | #F3F4EF | Dashboard background; service uses warmer #F8F8F1 |
| Teal | #006B60 | Brand anchor, progress and high-emphasis panels |
| Mint | #C4EDCE | Completed work, positive outcome |
| Coral / peach | #FF875F / #FFE1D2 | Attention and implementation category; blocked uses explicit red text |
| Lilac / pale lilac | #BCACF1 / #EAE3FC | Planning and supporting categories |
| Yellow / butter | #F4D35D / #FBEFBA | Focus, active navigation, in-progress work |
| Sky / pale sky | #A9D8F0 / #DEEFFA | Ready state and secondary categories |
| Danger | #94372D on #FFE1DB | Blocked/destructive actions, always labelled |

Aim for roughly 65% neutral surfaces, 25% light colour fields and 10% saturated accents. Use ink on light colours and white on deep teal. Saturated pastel accents are not suitable for small white text. Colour never replaces a status label or number. Category colours and status colours are separate concepts: use a category stripe or background and a labelled status chip.

## Typography and space

- Space Grotesk, weight 500–600: titles, numbers, prominent statements. Dashboard H1 26–32px; service H1 41–78px, depending on width.
- Manrope, 400–800: navigation, task text, forms and body. Dense dashboard body 12–14px, secondary labels 10–11px; service body 14–17px.
- Fallback: Segoe UI, Arial, sans-serif. Local embedded variable WOFF2 Latin subsets cover current English and Bahasa Melayu text. For Chinese/Tamil or other scripts, add a properly licensed script family; system fallback is available but not a finished multilingual design.
- Both fonts use SIL Open Font License 1.1. Notices are in FONT-LICENSES.txt. fonts.css is approximately 64KB before transport compression and makes no request to Google.
- Space scale: 4, 8, 12, 16, 24, 32, 48, 64px. Panels use 20–24px radii; controls 10–12px. Keep close items closer than unrelated groups.

## Components and composition

- One dominant panel per view. Dashboard: action panel beside progress. Service: headline beside an illustrative handoff. Avoid multiple competing hero treatments.
- Buttons: ink default, teal hover, pale secondary surfaces. Minimum primary/touch control height 44px; secondary desktop utilities may be 40px. Never add a decorative button that does nothing.
- Cards hold real groupings. Lists and dividers are preferable for repeated task detail; do not put every sentence into a card.
- Status mapping: planned neutral, ready sky, in progress butter, blocked peach/red, done mint/teal. Text labels remain mandatory.
- The progress dial is completed tasks / all tasks. It measures planning completion, never business health or financial performance.
- Forms: visible labels, clear borders, explicit results. Retain native validation and keyboard focus. Mailto preparation remains visibly distinct from sending.
- Artwork: code-native diagrams for process explanations. Use real photography only when it tells a verified story about actual people, work or place; obtain rights and consent.
- Motion: short colour/position transitions only; respect prefers-reduced-motion. Do not use motion to imply live activity.

## Responsive behaviour

Desktop: fixed labelled navigation, two-column summaries, four metrics, task boards with a contained horizontal scroller. Tablet: sidebar becomes a drawer at 900px; summary composition remains two columns until 680px. Phone: action and progress stack, metrics stay in two columns, task columns stack, forms precede role explanations. Service navigation collapses at 900px; hero becomes a single column at 650px. No essential control should require page-wide horizontal scrolling.

## Reuse in another project

1. Write one sentence defining audience, main action and emotional tone.
2. Copy relay-tokens.css and the applicable font assets/licences. Keep semantic token roles; choose the new brand anchor deliberately.
3. Select one or two supporting colour families. Retain status meaning, labels and sufficient contrast.
4. Choose the appropriate information density and original artwork. Do not automatically transplant NeatRelay copy, its N mark or founder details.
5. Build from the examples in design-system.html; inspect desktop, intermediate and phone widths with real content.
6. Check keyboard order, visible focus, menus, long titles, form errors, empty states, saved state, font fallback and reduced motion. Record results in that project's handover.

## Implementation map

`relay-tokens.css`: shared semantic values. `fonts.css`: locally embedded fonts. `relay-theme.css`: separate dashboard/service applications layered after their base styles. `design-system.html`: visual reference and interactive status specimen. Dashboard storage key and backup schema are unchanged. No UI backend or Trello sync was added.

Canonical source for shared files in the Astra Sandbox workspace: `focused/design-system/`. Identical copies of shared assets and this guide are published in both repositories. Edit the canonical files first and copy them to both sites to prevent drift.
