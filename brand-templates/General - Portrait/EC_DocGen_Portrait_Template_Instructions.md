# Evolving Consulting DocGen Portrait Template Library Instructions

## Purpose

These HTML files are reusable Letter-size portrait building blocks for creating branded Evolving Consulting documents in ChatGPT or Portwood DocGen.

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

## Available Portrait Templates

1. `EC_Master_Cover_Version_1_Portrait_URL.html`
2. `EC_Master_Cover_Version_2_Portrait_URL.html`
3. `EC_Master_Thank_You_Version_1_Portrait_URL.html`
4. `EC_Master_Thank_You_Version_2_Portrait_URL.html`
5. `EC_Master_Goals_Version_1_Portrait_URL.html`
6. `EC_Master_Goals_Version_2_Portrait_URL.html`
7. `EC_Master_Single_Column_Page_Portrait_URL.html`
8. `EC_Master_Two_Column_Page_Portrait_URL.html`
9. `EC_Master_Standard_Table_Portrait_URL.html`
10. `EC_Master_Four_Card_Page_Portrait_URL.html`
11. `EC_Master_Six_Card_Page_Portrait_URL.html`
12. `EC_Master_Process_Page_Portrait_URL.html`
13. `EC_Master_Image_Page_Portrait_URL.html`

## How to Use These in Claude

Use a request such as:

> Build a portrait Service Report using Cover Version 1, the Single-Column Page, the Standard Table, the Two-Column Page, and Thank You Version 1. Use the EC portrait master templates and preserve their image URLs, sizing, branding, fonts, and CSS conventions.

Or:

> Use `EC_Master_Process_Page_Portrait_URL.html` as the layout for the delivery process section. Keep it Letter portrait and replace only the sample text with the provided Salesforce merge tags.

## Rendering Rules

- Letter portrait: `@page { size: Letter portrait; margin: 0.70in; }`
- Arial with Helvetica fallback.
- Use `<table>`, `<tr>`, and `<td>` for structural layouts.
- Do not use flexbox, CSS grid, `gap`, `calc()`, CSS variables, transforms, gradients, SVG, JavaScript, or web fonts.
- Use solid colors only.
- Keep image dimensions explicit.
- Use a real `<thead>` for repeating table headers.
- Place child-loop opening and closing tags inside the row that repeats.
- Avoid fixed heights for long-text sections.
- Use `page-break-inside: avoid` only for compact cards, short tables, and process steps.
- Avoid unnecessary forced page breaks between flowing legal or long-text sections.



## Template Selection

- Cover Version 1: centered executive cover.
- Cover Version 2: editorial cover with a black information panel.
- Thank You Version 1: large left-aligned closing page with a bottom-right contact panel.
- Thank You Version 2: centered formal closing page.
- Goals Version 1: simple numbered agenda.
- Goals Version 2: agenda plus supporting panel.
- Single-Column Page: long descriptions, objectives, assumptions, summaries, and legal content.
- Two-Column Page: comparisons, responsibilities, assumptions and exclusions, or business and technical details.
- Standard Table: repeating Salesforce child records and totals.
- Four-Card Page: four metrics or strategic highlights.
- Six-Card Page: services, guidance, recommendations, or responsibilities.
- Process Page: vertical five-step process.
- Image Page: screenshot, workflow, diagram, or other supporting visual.

## Important

When creating a new document from these templates, preserve the page size, Arial font, EC branding, image URLs, spacing principles, and Flying Saucer-compatible CSS unless the user explicitly approves a change.
