---
name: FastAPI Blog
description: A tutorial-built blog about FastAPI and Python web development, presented by Briva Digital
colors:
  stormfront-steel: "#527c9f"
  steel-deep: "#466a87"
  steel-deeper: "#3f6179"
  tide-link: "#428bca"
  mist-link: "#cbd5db"
  workshop-paper: "#fafafa"
  bench-white: "#ffffff"
  graphite-ink: "#333333"
  heading-ink: "#444444"
  hairline-border: "#dddddd"
  hairline-faint: "#e3e3e3"
  ember-danger: "#a85b5b"
  ember-danger-deep: "#924e4e"
  moss-success: "#4a7c5d"
  steel-moonlight: "#8aadc8"
  night-sky: "#1a1a1a"
  bench-night: "#2d2d2d"
  moonlit-ink: "#e0e0e0"
  moonlit-heading: "#f0f0f0"
  night-hairline: "#404040"
  night-hairline-faint: "#4a4a4a"
typography:
  heading:
    fontFamily: "Montserrat, system-ui, -apple-system, BlinkMacSystemFont, sans-serif"
    fontWeight: 500
  body:
    fontFamily: "Nunito, system-ui, -apple-system, BlinkMacSystemFont, sans-serif"
    fontSize: "1rem"
    lineHeight: 1.5
  article-body:
    fontSize: "1.25rem"
rounded:
  sm: "0.375rem"
  md: "0.5rem"
  full: "50%"
spacing:
  card-y: "1rem"
  card-x: "1.5rem"
  stack: "1.5rem"
  xl: "5rem"
components:
  button-primary:
    backgroundColor: "{colors.stormfront-steel}"
    textColor: "#ffffff"
    rounded: "{rounded.sm}"
    padding: "0.375rem 0.75rem"
  button-primary-hover:
    backgroundColor: "{colors.steel-deep}"
    textColor: "#ffffff"
  card:
    backgroundColor: "{colors.bench-white}"
    textColor: "{colors.graphite-ink}"
    rounded: "{rounded.md}"
    padding: "1rem 1.5rem"
  card-dark:
    backgroundColor: "{colors.bench-night}"
    textColor: "{colors.moonlit-ink}"
  navbar:
    backgroundColor: "{colors.stormfront-steel}"
    textColor: "{colors.mist-link}"
---

# Design System: FastAPI Blog

## Overview

**Creative North Star: "The Well-Kept Workshop"**

This is a public workshop where learning happens in the open: honest tools arranged on a tidy bench, zero pretension, everything built to be used. The visual system reads as calm and studious — closer to good documentation than to a product launch. A Bootstrap chassis is used without apology; the identity comes from two disciplined choices kept constant everywhere: the Stormfront Steel navigation rail and the Montserrat/Nunito type pairing.

Surfaces are plain paper on a desk. Cards carry a hairline border and a whisper of shadow at rest, and depth appears only when the reader touches something — a lift on hover, never a permanent status symbol. Color is rationed like paint in a shop: one steel-blue voice owns structure and primary actions, semantic colors stay dusty rather than alarmed, and everything else is graphite ink on white paper. Dark mode simply moves the same workshop indoors: warmer-than-black surfaces, the steel rail unchanged.

Confirmed anti-reference: no SaaS launch gloss. No gradient hero banners, glow shadows, or glassmorphism — this is a working bench, not a pitch deck.

**Key Characteristics:**
- Fixed Stormfront Steel navbar that survives both themes unchanged
- Two fonts only: Montserrat speaks (headings), Nunito works (body)
- Flat-at-rest surfaces; shadow exclusively as interaction feedback
- Hairline-bordered cards (0.5rem radius) on near-white paper (#fafafa)
- Dusty semantic palette: ember red (#a85b5b), moss green (#4a7c5d) — never alarm colors
- Round avatars ringed in the surface color they sit on
- First-class light/dark/auto theming persisted across visits

## Colors

A near-monochrome workshop: graphite inks on paper whites, one structural steel blue, and two muted semantic accents.

### Primary
- **Stormfront Steel** (#527c9f): The single brand voice. Owns the fixed navigation rail, primary buttons, and the browser theme-color. It is structure, not decoration — if steel appears somewhere with nothing to hold up, it shouldn't be there. Hovers deepen to Steel Deep (#466a87), active presses to Steel Deeper (#3f6179).
- **Steel Moonlight** (#8aadc8): The same steel lifted for dark mode, where filled steel would glare. Used for primary-button text/borders on dark surfaces.

### Secondary
- **Ember Danger** (#a85b5b): Destructive actions only — delete buttons and the danger modal header. Deliberately dusty brick, not Bootstrap alarm-red; deepens to #924e4e on hover. In dark mode it lifts to #d89090 with dark text.
- **Moss Success** (#4a7c5d): Confirmation moments, currently the success modal header. Same dust-and-moss restraint as Ember.

### Neutral
- **Workshop Paper** (#fafafa): Page background. Never pure white — the bench has a tooth to it.
- **Bench White** (#ffffff): Card and content-section surfaces sitting on the paper. Becomes Bench Night (#2d2d2d) after dark.
- **Graphite Ink** (#333333): Body text. Moonlit Ink (#e0e0e0) in dark mode.
- **Heading Ink** (#444444): All headings; one step lighter than body ink to soften large type. Moonlit Heading (#f0f0f0) in dark mode.
- **Hairline Border** (#dddddd) / **Hairline Faint** (#e3e3e3): The workshop's joinery — card edges, metadata dividers, footer rule. Night Hairline (#404040) / (#4a4a4a) in dark mode.
- **Mist Link** (#cbd5db): Nav links resting on the steel rail, brightening to white on hover/focus.
- **Tide Link** (#428bca): Interactive text accent — article-title hovers and all keyboard focus rings. The only cool blue allowed outside steel.

### Named Rules
**The One Steel Rule.** Stormfront Steel is the only brand color, and it always does structural work — the rail, primary actions. Nothing else competes for it, and it never appears as passive decoration.

**The Dusty Semantic Rule.** Semantic colors arrive pre-muted: danger is #a85b5b, success is #4a7c5d. Reaching for saturated framework reds and greens breaks the workshop's voice.

## Typography

**Display Font:** Montserrat (variable 100–900, with system-ui fallbacks)
**Body Font:** Nunito (variable 200–1000, with system-ui fallbacks)

**Character:** A geometric sans speaking over a humanist sans working — Montserrat gives headings a composed, slightly formal voice while Nunito's rounded warmth keeps long reading friendly. Together they read studious, not corporate.

### Hierarchy
- **Heading** (Montserrat 500, Bootstrap's h-scale — h2 ≈ 2rem, h1 up to 2.5rem): Every h1–h6 plus the navbar brand. Headings share Heading Ink (#444444).
- **Article Body** (Nunito 400, 1.25rem, rendered with `white-space: pre-line`): Post content sits a step larger than UI text because reading is the point; author line breaks are honored literally.
- **Body** (Nunito 400, 1rem, 1.5 line-height): Default UI text — card copy, sidebar, footer.
- **Metadata** (Nunito small/text-secondary, 400): Author names and dates under the hairline; quiet by design.

Bootstrap supplies the scale; this system supplies the families and the discipline of not adding a third.

### Named Rules
**The Two-Hand Rule.** Montserrat speaks, Nunito works. No third font ever joins the bench — no monospace accents, no serif flourishes.

## Layout

A centered Bootstrap container holds a two-column reading layout: the article stream takes two-thirds (`col-md-8`), a sidebar panel takes one-third (`col-md-4`), collapsing to a single column below the 768px breakpoint. A fixed navbar sits above everything; pages compensate with 5rem of top padding on `main` — the one large, non-negotiable spatial commitment. Articles stack vertically with 1.5rem between cards, each card padded 1rem vertically and 1.5rem horizontally. The footer sticks to the viewport floor via a flex-column body (`mt-auto`), holding a centered, muted copyright line whose year is set by script.

Density is comfortable, not dense — whitespace is generous around the reading column and tighter inside cards. Mobile keeps the same vertical rhythm; the navbar folds into a Bootstrap collapse with Login/Register dropping to full-width rows.

## Elevation & Depth

Depth here is feedback, not hierarchy. Surfaces lie flat against the paper at rest — a card is distinguished by its hairline border and one shade of separation, not by floating. When the reader reaches toward a card (hover/focus), it lifts: the shadow deepens and the border warms a step. Dark mode runs heavier, tighter shadows because low-contrast edges need them. Avatars get a 2px ring in their own surface color — a punched hole in the card, not a drop shadow.

### Shadow Vocabulary
- **Card at rest** (`box-shadow: 0 2px 4px rgba(15, 23, 42, 0.05)`): Barely-there grounding for `.content-section` surfaces.
- **Card lift** (`box-shadow: 0 4px 10px rgba(15, 23, 42, 0.1)`): Hover response, paired with border shift to Hairline Faint and a 0.15s ease transition.
- **Night rest / night lift** (`0 1px 3px rgba(0, 0, 0, 0.3)` / `0 2px 8px rgba(0, 0, 0, 0.5)`): Dark-mode equivalents — stronger but smaller-radius, keeping lift legible without glow.
- **Avatar ring** (`box-shadow: 0 0 0 2px var(--color-bg-content)`): Circular profile images; a flat ring, never a shadow.

### Named Rules
**The Paper-on-a-Desk Rule.** Resting surfaces are flat. Shadow exists only as a response to touch (hover, focus) — a shadow at rest with no interaction attached is a defect.

## Shapes

Soft-edged but square-shouldered. Cards round at 0.5rem, buttons and inputs at Bootstrap's 0.375rem — a consistent family of gentle corners, never pill-shaped except for true circles: avatars are cut at 50% and ringed in their surface color. Borders do the separating work before shadows do: 1px hairlines edge every card, divide the article-metadata strip, and cap the footer. There is no clipping, no skewed geometry, no ornament — the recurring silhouette is a plain rectangle with quietly rounded shoulders, exactly what a well-kept bench looks like.

## Components

### Buttons
- **Shape:** Gentle rectangle, 0.375rem radius; Bootstrap sizing (0.375rem × 0.75rem padding).
- **Primary:** Solid Stormfront Steel fill (#527c9f) with white text; hovers deepen to #466a87, active to #3f6179. In dark mode, primary flips to outline style: Steel Moonlight (#8aadc8) text/border, filling with dark text on hover.
- **Danger:** Outline style at rest — Ember (#a85b5b) text and border on transparent; fills dusty-to-deeper (#924e4e) on press. Used for Delete actions only.
- **Secondary/Nav:** On the steel rail, actions are `btn-outline-light` (Login) and `btn-light` (Register) — inverted paper chips riding the rail.
- **Hover / Focus:** 0.15–0.2s ease transitions; every control shows a visible keyboard ring (2px solid #428bca, 2px offset).

### Navigation
Fixed-top rail in Stormfront Steel, forced to its own dark palette (`data-bs-theme="dark"`) regardless of page theme — it never changes. Brand wordmark in Montserrat; links in Mist (#cbd5db) brightening to white, active weight 600. Right side carries Login/Register chips and the theme dropdown (🌝 Light / 🌚 Dark / 🌛 Auto, persisted in `localStorage`). Under 768px the whole right side collapses behind a toggler.

### Cards / Containers
`.content-section` is the universal container: Bench White surface, 1px Hairline Border, 0.5rem radius, rest shadow, 1rem/1.5rem padding, lift on hover. The sidebar wraps the same container around a Bootstrap list-group.

### Article Card (signature component)
The repeating unit of the site: 64px circular avatar (48px mobile) ringed in Bench White on the left; right side stacks a metadata strip (author link + date) sealed by a hairline underline, an h2 title in Heading Ink that shifts to Tide Link (#428bca) on hover, then 1.25rem body copy with preserved line breaks. It demonstrates every rule in the system at once: flat rest state, hairline joinery, rationed color, responsive lift.

### Inputs / Fields
Bootstrap form-controls at 0.375rem radius on Bench White with hairline borders; a compact `.file-input-sm` (300px max) exists for upload fields. Focus follows the global ring. Full form flows arrive with authentication — extend these defaults, don't replace them.

### Dialogs
Bootstrap modals for confirmation (Delete Post). Colored-header variant available: Moss Success or Ember Danger header bands carrying white titles in both themes. Copy is plain-spoken ("Are you sure… This action cannot be undone.") — keep it that way.

## Do's and Don'ts

### Do:
- **Do** keep the navbar Stormfront Steel (#527c9f) in both themes — it is the system's one constant rail.
- **Do** pair Montserrat headings with Nunito body text, loaded once from Google Fonts.
- **Do** show a visible focus ring on every interactive element (`outline: 2px solid #428bca; outline-offset: 2px`).
- **Do** render post bodies at 1.25rem with `white-space: pre-line` — author line breaks are content.
- **Do** move dark mode indoors gradually: #1a1a1a page, #2d2d2d surfaces, #404040 hairlines.

### Don't:
- **Don't** use gradient text, neon glow shadows, frosted glass, or animated hero banners — no SaaS launch gloss anywhere.
- **Don't** reach for saturated framework reds/greens; semantic color stays dusty (danger #a85b5b, success #4a7c5d).
- **Don't** put shadows on resting surfaces — lift is a response to touch, per the Paper-on-a-Desk Rule.
- **Don't** introduce a third font, pill-shaped buttons, or pure black (#000) backgrounds.
