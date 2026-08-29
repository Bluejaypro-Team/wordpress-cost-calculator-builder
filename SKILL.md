---
name: wordpress-cost-calculator-builder
description: >-
  Generates production-grade, highly localized, copy-and-paste WordPress cost calculators (HTML/CSS/JS)
  based on minimal user inputs (Location, Calculator Keyword, Color Codes, Font Family, Container Width).
  Includes deep logo color extraction, mandatory centered titles, strict #FFFFFF background, 3-factor input mode,
  5-second auto-close/minimize results card with hover pause, itemized line items, visual stacked breakdown bar,
  click-to-call consultation CTA, print PDF support, and automated minification.
---

# Global WordPress Cost Calculator Builder Skill

This skill provides an autonomous end-to-end framework to build high-converting, localized, standalone WordPress cost calculator widgets for any trade, service, product, or industry.

---

## 1. Mandatory Design & Branding Directives (STRICT ENFORCEMENT)

When creating, updating, or generating any WordPress cost calculator, ALWAYS enforce the following strict rules:

### A. Deep Logo Color Analysis & Dual-Color Harmony
- **Visual Inspection**: Thoroughly inspect the target website's logo image and extract the exact primary and secondary color palette (Hex codes).
- **Brand System**:
  - **Primary Logo Color**: Apply to primary action buttons, active tab/segmented pill backgrounds, header titles, focus borders, and main breakdown bar segments.
  - **Secondary Logo Color**: Apply to active pill bottom accent indicators (`border-bottom: 3px solid`), secondary borders, badge highlights, legend tags, and CTA accents.

### B. Centered Header Section (STRICT MANDATE)
- **Centering**: The header block (Location Badge, Main Calculator Title, Subtitle, and Gold Gradient Divider) **MUST ALWAYS be centered** (`text-align: center; margin: 0 auto;`).
- **Forbidden**: NEVER left-align or right-align the top calculator header title block.

### C. Calculator Container Background (STRICT MANDATE)
- **Background Color**: You MUST **ONLY use `#FFFFFF`** (Pure White) as the background color code for all calculator containers (`background: #FFFFFF;` or `--card-bg: #FFFFFF;`).
- **Forbidden**: NEVER use grey (`#F8FAFC`, `#F1F5F9`), dark, or tinted backgrounds for the main calculator container box.

### D. Universal Container Bounds
- **Container Max-Width**: Default MUST ALWAYS be `max-width: 100%` for fluid, flawless responsive rendering across PC header right areas, sidebars, body contents, and mobile viewports.

---

## 2. Minimal User Inputs Required

When the user provides minimal input, extract or request the following key variables:

| Input Variable | Description / Example | Default Value (If Unspecified) |
| :--- | :--- | :--- |
| **Location** | City, Zip, or Region (e.g., `Antelope, CA`) | `Antelope, CA` (COLA: 1.15x) |
| **Calculator Keyword** | Target SEO Keyword (e.g., `ADU Design Build Cost`) | Prompt or infer from user context |
| **Color Palette** | Primary & Secondary Logo Hex Codes | Extracted from logo image |
| **Font Family** | Google Font or standard font stack | `'Open Sans', sans-serif` |
| **Container Width** | Max-width constraint for fluid responsive layout | `max-width: 100%` |

---

## 3. Standard Operational Workflow

```mermaid
flowchart TD
    A["1. User Request & Logo Analysis"] --> B["2. Web Search & Local Rate Grounding"]
    B --> C["3. Python Math Test Harness & Verification"]
    C --> D["4. Generate Formatted HTML/CSS/JS Snippet"]
    D --> E["5. Generate Minified WordPress Copy-Paste Code"]
```

### Step 1: Web Search & Local Rate Grounding
Use `search_web` to retrieve localized cost metrics for the target keyword in the specified location:
- Local Trade Labor Hourly Rate (e.g., Glazier/Electrician/Plumber/General Contractor labor baseline).
- Material Unit Rates (Base materials, premium tiers, addons).
- Local Building Codes & Climate Standards (e.g., California Title 24, SB 13 impact fee exemptions under 750 sq.ft.).
- Ancillary Fees (Demolition, disposal, permits, specialized engineering).

### Step 2: Math Verification via Python Test Harness
Create a python script in scratch (e.g., `verify_[service]_calculator.py`) using `write_to_file`, then execute it using `run_command`:
- Verify all formula outputs, range bounds (Min: -10%, Max: +12%), unit subtotals, and edge cases.
- Confirm Exit Code 0 before generating frontend HTML code.

### Step 3: Standalone WordPress Code Generation (`-snippet.html`)
Build a 100% self-contained module containing:
1. **Centered Header**: Location badge, title, subtitle, and gradient line centered.
2. **Streamlined 3-Factor Input Controls**:
   - Factor 1: ADU / Project Type (Horizontal Segmented Pill Buttons)
   - Factor 2: Size / Scope (Interactive Slider with live impact fee waiver badge)
   - Factor 3: Finish Quality Tier (Pill Selector: Standard, Custom, Luxury)
3. **Ultra-Simple & High-Impact Results Display**:
   - Hero Price Display: Huge bold total investment price, range tag, and unit rate.
   - Clean 4-Line Item Breakdown: Itemized list with icons, descriptions, and subtotals.
   - Phone CTA Banner: Click-to-call contact box for direct lead conversion (`📞 Call (916) 555-0199 Now`).
4. **Interactive 5-Second Auto-Close Results Box**:
   - Initial state: `style="display: none;"`
   - Trigger: Clicking **"🧮 Calculate [Service] Cost"** displays card, scrolls smoothly into view, and starts 5s countdown.
   - Hover Pause: `mouseenter` pauses countdown, `mouseleave` resumes.
   - Manual Close: Includes `✖ Minimize / Close` button.

### Step 4: Automated Minification Pipeline (`-minified.html`)
Write a python minification script (e.g., `minify_[service].py`) that strips comments and unnecessary whitespace from HTML, CSS, and JS. Run via `run_command` and present both Option 1 (Minified Code) and Option 2 (Formatted Code).

---

## 4. Standardized Multi-Vector Pricing Formula

$$\text{Total Investment} = \left[ \left( \text{Base Material Rate} \times \text{Quantity/Area} \times \text{Finish Multiplier} \right) + \text{Design Cost} + \text{Utility Cost} + \text{Permit Fee} \right] \times \text{Regional COLA Multiplier}$$

Where:
- **Min Estimate**: $\text{Total} \times 0.90$
- **Max Estimate**: $\text{Total} \times 1.12$
- **Unit Metric**: $\text{Total} / \text{Quantity or Sq.Ft.}$

---

## 5. Output Deliverable Formatting Guide

When presenting the output to the user, always provide:
1. **Option 1: Compressed / Minified WordPress Code**: Wrapped in a single ````html ```` block ready for copy-pasting into Gutenberg / Elementor / Divi.
2. **Option 2: Formatted Code**: Cleanly indented code with inline comments for users who wish to customize field options or pricing constants.
3. **Local Scratch File References**: Links to `[service]-snippet.html` and `[service]-minified.html`.
