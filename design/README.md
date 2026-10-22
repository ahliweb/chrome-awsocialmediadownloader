# Design assets

Source files for the popup design and the backlog analysis of this repository. The specification they illustrate is [`docs/UX.md`](../docs/UX.md) (issue #6).

## Format

Each `*.dc.html` file is one artboard of a Claude Design canvas. `canvas.json` is the canvas index: frame positions, pages, notes, and the artboard order.

The artboards load a `./support.js` runtime that is provided by the canvas editor and **is not part of this repository**. Opened directly in a browser, they render as plain HTML with layout and styling intact, but template bindings and links between artboards will not work.

These files are design references only. They are not shipped in the extension package; #12 package validation must keep `design/` out of the zip.

## Popup (page "UI/UX ekstensi")

| File | State | `UI-*` |
|---|---|---|
| `S1-Pemberitahuan.dc.html` | S1 · Rights notice, first run | UI-001, UI-003 |
| `S2-BukanFacebook.dc.html` | S2 · Not on Facebook | UI-002, UI-005 |
| `S3-BelumAdaMedia.dc.html` | S3 · No media yet | UI-006 |
| `S4-DaftarMedia.dc.html` | S4 · Media list (single files) | UI-007, UI-008 |
| `S5-TrekTerpisah.dc.html` | S5 · Separate video and audio tracks | UI-009 |
| `S6-Mengunduh.dc.html` | S6 · Downloading and done | UI-010 |
| `S7-Galat.dc.html` | S7 · Error: expired link | UI-011 |
| `S8-Gelap.dc.html` | Variant · Dark mode with visible focus ring | UI-013 |
| `S9-English.dc.html` | Variant · English locale | UI-012 |
| `Toko-Screenshot.dc.html` | Chrome Web Store screenshot 1280 × 800 (#18) | — |
| `Alur.dc.html` | Interaction flow | — |
| `Spesifikasi.dc.html` | Visual spec: tokens, `UI-*` table, copy table, accessibility | — |

Mockup copy is in Indonesian, except `S9-English`. All copy is defined in English and Indonesian in `docs/UX.md` §5. Sample video titles are placeholders.

## Backlog analysis (page "Analisis isu")

Snapshot of the 18 open issues taken on 2026-10-23.

| File | Content |
|---|---|
| `Main.dc.html` | Summary: counts, priority and phase distribution, key findings |
| `Risiko.dc.html` | Risk matrix and register, cross-issue inconsistencies, priority actions |
| `Graf.dc.html` | Dependency graph and critical path (#2 → #3 → #5 → #7 → #8 → #10 → #11 → #12 → #17 → #18) |
| `Standar.dc.html` | Mapping of issues to ISO/IEC standards, Indonesian and international regulation, and precedents |

The analysis is a point-in-time assessment, not legal advice. Compliance decisions remain with the owner in #4.
