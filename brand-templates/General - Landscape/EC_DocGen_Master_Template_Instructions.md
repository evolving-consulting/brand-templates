# Evolving Consulting DocGen Template Library Instructions

## Purpose

These HTML files are reusable landscape Letter-size building blocks for creating branded Evolving Consulting documents in ChatGPT or Portwood DocGen.

## Branding Images

Use these URLs exactly unless a newer approved URL is provided:

- EC Cube:`https://ec-website.mnava.workers.dev/email-signature/icon-cube-teal.png`
- EC Logo: `https://ec-website.mnava.workers.dev/email-signature/logo-lockup.png`

## Color Palette

Use these hex values for all branded document colors:

| Role | Hex |
|---|---|
| Accent teal (light) | `#1f5f5b` |
| Accent teal (dark) | `#69b8ae` |
| Ink (text/dark backgrounds) | `#14161a` |
| Body text | `#31363a` |
| Muted text | `#6b736e` |
| Hairline (borders/dividers) | `#dde2dc` |
| Background | `#f3f5f2` |
| Accent soft (teal-tinted light panel) | `#e6efee` |
| Accent bright (on-dark label color) | `#69b8ae` |

Use solid colors only — no gradients. `#e6efee` is the standard light panel background used in DocGen templates.

## Available Landscape Templates

1. `EC_Master_Cover_Version_1_Landscape_URL.html`
2. `EC_Master_Cover_Version_2_Landscape_URL.html`
3. `EC_Master_Thank_You_Version_1_Landscape_URL.html`
4. `EC_Master_Thank_You_Version_2_Landscape_URL.html`
5. `EC_Master_Goals_Version_1_Landscape_URL.html`
6. `EC_Master_Goals_Version_2_Landscape_URL.html`
7. `EC_Master_Single_Column_Page_Landscape_URL.html`
8. `EC_Master_Two_Column_Page_Landscape_URL.html`
9. `EC_Master_Standard_Table_Landscape_URL.html`
10. `EC_Master_Four_Card_Page_Landscape_URL.html`
11. `EC_Master_Six_Card_Page_Landscape_URL.html`
12. `EC_Master_Process_Page_Landscape_URL.html`
13. `EC_Master_Image_Page_Landscape_URL.html`

## How to Request a Document in Claude

Use a request such as:

> Build a landscape Project Status document using Cover Version 1, the Four-Card Page, the Standard Table, the Two-Column Page, and Thank You Version 1. Use the EC master branding and the provided Salesforce merge tags.

Or:

> Use `EC_Master_Process_Page_Landscape_URL.html` as the layout for this section. Keep the existing image URLs, sizing, fonts, and CSS conventions.

## Required Rendering Rules

- Letter landscape: `@page { size: Letter landscape; margin: 0.75in; }`
- Arial with Helvetica fallback.
- Use tables, table rows, and table cells for layout.
- Do not use flexbox, CSS grid, `gap`, `calc()`, transforms, gradients, SVG, JavaScript, or web fonts.
- Use solid colors only.
- Keep image dimensions explicit.
- Use a real `<thead>` for repeating table headers.
- Place child-loop opening and closing tags inside the row that repeats.
- Avoid fixed heights for long-text sections.
- Use `page-break-inside: avoid` only for cards, short tables, and compact components.
- Do not force unnecessary page breaks between flowing legal or long-text sections.



## Template Selection Guide

- Cover Version 1: centered executive cover.
- Cover Version 2: editorial cover with a black information panel.
- Thank You Version 1: large left-aligned closing page with a bottom-right contact panel.
- Thank You Version 2: centered formal closing page.
- Goals Version 1: simple numbered agenda.
- Goals Version 2: agenda with a supporting information panel.
- Single-Column Page: long text, legal language, objectives, assumptions, or summaries.
- Two-Column Page: comparisons, responsibilities, assumptions and exclusions, or business and technical details.
- Standard Table: repeating Salesforce child records and totals.
- Four-Card Page: four metrics or strategic highlights.
- Six-Card Page: services, recommendations, responsibilities, or guidance.
- Process Page: five-step delivery or business process.
- Image Page: screenshot, diagram, workflow, or visual with explanatory text.

## Important

When creating a new document from these templates, preserve the EC branding, page size, font, image URLs, spacing principles, and Flying Saucer-compatible CSS unless the user specifically approves a change.
