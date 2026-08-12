# Intra-Zone vs Inter-Zone Call Flow

IMS solution doc (v17.0) that diagrams SIP call signaling for two scenarios on the IMS core — an **intra-zone** call, where both subscribers sit under the same Main DC, and an **inter-zone** call, where the call crosses zones through IBCF/GMSC interconnect. It shows which nodes (P-CSCF, I/S-CSCF, TAS, IMSENUM, HSS/SLF, IBCF, MRF, IMS-DP, etc.) are involved at each phase — origination, number resolution, interconnect, termination, and answer/media — which interfaces (Gm, Mw, ISC, Cx, Sh, ENUM, Rx, IBCF trunk) carry each message, and exactly where the two flows diverge.

## Contents

- **`index.html`** — homepage, currently a copy of the v2 document.
- **`IMS Call Flow v2.dc.html`** — latest version of the call flow doc.
- **`IMS Call Flow.dc.html`** — original version.
- **`support.js`** — shared runtime that renders the `<x-dc>` document format used by both HTML files (do not edit directly; see note in the file header).
- **`screenshots/`, `uploads/`** — reference images, not linked from the documents.

## Viewing locally

These are static, self-contained HTML files with no build step. Open `index.html` directly in a browser, or serve the folder:

```bash
npx serve .
```

## Deployment

Configured for static hosting on [Netlify](https://www.netlify.com) — see `netlify.toml` (publish directory is the project root, no build command required).
