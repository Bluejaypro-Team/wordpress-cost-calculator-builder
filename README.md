# WordPress Cost Calculator Builder Skill

An autonomous AI agent skill to generate production-grade, highly localized, standalone copy-and-paste WordPress cost calculator widgets (HTML/CSS/JS) optimized for header right, desktop, tablet, and mobile viewports based on minimal user inputs.

## 📌 Core Architecture & Standards

- **Title-Only Centered Header**: Clean, focused header with centered title only (`<h2 class="bcc-title">...</h2>`). Location badges and subtitles are revoked to eliminate vertical bloat and fit header right columns.
- **Strict #FFFFFF Background**: Mandatory `#FFFFFF` (Pure White) background across all containers and modals.
- **All-Dropdown Text-Type Architecture**: Multi-choice options (methods, materials, access) are built using standard `<select>` inputs with option labels strictly < 35 characters to prevent clipping in narrow header-right columns.
- **Theme-Immune Styling**: Complete reset (`all: unset !important; box-sizing: border-box !important;`), 42px height, 40px line-height, zero vertical padding, custom SVG chevron arrows.
- **Container Query & 2-Column Grid**: `container-type: inline-size;` collapses from 2 columns to 1 column on narrow containers (< 380px) and mobile (< 440px).
- **Hidden Stepper Protocol**: Custom square footage stepper is hidden by default and toggles on demand.
- **Anti-Cascade Specificity Lightbox**: Results popup with Astra-immune circular close button (30px x 30px, `border-radius: 50% !important;`), 5-second auto-close countdown with hover pause (`bccPauseTimer` / `bccResumeTimer`), proportional cost bar, and itemized specs table.
- **Direct Lead Conversion**: Dual side-by-side action CTAs ("Book Free Site Walk" / Contact URL + "Call Now" click-to-call) with CSLB / municipal license compliance note.
- **Revoked Print Bloat**: Unneeded generic PDF print buttons and iframe injection scripts are omitted to maximize lead conversion speed and reduce snippet payload.
- **100% Valid Single-Root Schema**: 5-entity `@graph` JSON-LD (`WebSite`, `WebPage`, `WebApplication`, `Service`, `GeneralContractor`).
- **Automated Minification**: Python pipeline generating single-block production snippets.

## 🛠️ Minimal Inputs Required

- **Location**: Target city & state (e.g., `Sacramento, CA`)
- **Calculator Keyword**: Target SEO Keyword (e.g., `Swimming Pool Demolition Cost Calculator`)
- **Website URL & Contact**: Company website URL and `/contact-us/` booking endpoint
- **Company Name & License**: Legal business name and contractor license (e.g., CSLB C-21)
- **Direct Phone**: Click-to-call phone number (e.g., `+19163185272`)

## 📄 License

MIT License
