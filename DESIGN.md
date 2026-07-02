---
name: AI Vocabulary × UX Research — Mind-map
description: A single-page mind-map for browsing AI/LLM vocabulary through a UX-research lens.
colors:
  indigo-focus: "#4f46e5"
  indigo-weak: "#eef2ff"
  indigo-deep: "#3730a3"
  teal-status: "#0f766e"
  teal-status-bg: "#ecfdf5"
  teal-status-border: "#ccfbf1"
  badge-border: "#dbeafe"
  highlight-amber: "#fef3c7"
  hero-gradient-start: "#111827"
  hero-gradient-end: "#312e81"
  neutral-bg: "#f5f7fb"
  surface: "#ffffff"
  surface-soft: "#f9fafb"
  ink: "#111827"
  body-text: "#344054"
  tag-text: "#475467"
  muted: "#667085"
  muted-2: "#8a94a6"
  border: "#e5e7eb"
  border-strong: "#cbd5e1"
typography:
  display:
    fontFamily: "Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "clamp(28px, 3vw, 44px)"
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "28px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.04em"
  title:
    fontFamily: "Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "24px"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "-0.035em"
  body:
    fontFamily: "Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "normal"
  label:
    fontFamily: "Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "12px"
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: "0.08em"
rounded:
  pill: "999px"
  sm: "14px"
  md: "16px"
  lg: "18px"
  xl: "22px"
  2xl: "28px"
spacing:
  xs: "6px"
  sm: "12px"
  md: "14px"
  lg: "18px"
  xl: "26px"
  2xl: "32px"
components:
  button-primary:
    backgroundColor: "{colors.indigo-focus}"
    textColor: "#ffffff"
    rounded: "{rounded.sm}"
    padding: "12px 14px"
  input-search:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "12px 14px"
  nav-branch-button:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "12px"
  nav-branch-button-active:
    backgroundColor: "{colors.indigo-weak}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "12px"
  term-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: "14px 14px 13px"
  pill-status:
    backgroundColor: "{colors.teal-status-bg}"
    textColor: "{colors.teal-status}"
    rounded: "{rounded.pill}"
    padding: "5px 9px"
  pill-badge:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.indigo-deep}"
    rounded: "{rounded.pill}"
    padding: "2px 8px"
  chip-related:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.body-text}"
    rounded: "{rounded.pill}"
    padding: "7px 10px"
---

# Design System: AI Vocabulary × UX Research — Mind-map

## 1. Overview

**Creative North Star: "The Research Desk"**

The system reads like a well-organized research desk: a dark indigo header announces the workspace, then everything underneath drops into calm, flat, near-white panels with a single soft ambient shadow. One typeface (Inter) carries every role from hero to label; hierarchy comes entirely from size, weight, and tight negative tracking rather than a second font or decorative treatment. Two accents do all the signaling — indigo for focus/selection, teal for status counts — and nothing else in the interface is allowed to mean something visually.

This baseline explicitly rejects the generic "AI SaaS" scaffolding: no gradient text, no cream/sand backgrounds, no tiny uppercase tracked eyebrows, no numbered section markers as decoration. The term-card grid is a deliberate exception to "cards are the lazy answer" — the content genuinely is a set of parallel, browsable items, which is the one case a card grid earns its place.

**Known gap, stated plainly:** PRODUCT.md sets the target personality as "warm & approachable," but this indigo/slate system reads as calm and precise, not warm. That's an accurate description of what's built today, not an endorsement — closing that gap is follow-up work (see Do's and Don'ts), not something to retrofit into this document by inventing colors that aren't implemented.

**Key Characteristics:**
- Dark indigo hero band against otherwise flat, near-white panels
- Single sans-serif (Inter) across all five typographic roles
- Two meaningful accents only: indigo (focus/selection) and teal (status/count)
- Pill shape (999px) reserved exclusively for status/meta chips
- Flat surfaces at rest; one ambient shadow role, no shadow escalation on hover

## 2. Colors

A cool, restrained palette: two accent hues carrying meaning, everything else neutral.

### Primary
- **Indigo Focus** (`#4f46e5`): the only color that means "active, selected, or interactive focus." Used on the active nav button's tint, the search/select focus ring, the primary button fill, and the active term card's focus ring.

### Secondary
- **Teal Status** (`#0f766e`): the only color that means "status or count," never selection. Used on the mode pill text (paired with `#ecfdf5` background / `#ccfbf1` border).

### Tertiary
- **Indigo Deep** (`#3730a3`): a darker indigo reserved for small label text on light indigo-tinted chips (the cluster badge, the detail panel's cluster pill) — never used as a fill.
- **Highlight Amber** (`#fef3c7`): reserved exclusively for `<mark>` search-term highlighting. It has no other job in the system.

### Neutral
- **Neutral Bg** (`#f5f7fb`): page background, warmed only by a faint radial indigo glow (`#eef2ff` fading to transparent) top-left.
- **Surface** (`#ffffff`): all panels, cards, and controls sit on pure white.
- **Surface Soft** (`#f9fafb`): the counter pill and tag backgrounds — one step off white, for meta-level chrome.
- **Ink** (`#111827`): primary text and the hero's dark gradient start.
- **Body Text** (`#344054`): detail-panel paragraph copy and related-term chip labels — a half-step lighter than Ink for long-form reading.
- **Tag Text** (`#475467`): the smallest, quietest label color, used only on `.tag`.
- **Muted** (`#667085`) / **Muted 2** (`#8a94a6`): descriptive copy (branch descriptions, card subtitles) and section-label color respectively.
- **Border** (`#e5e7eb`) / **Border Strong** (`#cbd5e1`): default hairline vs. the emphasized/dashed border used on hover states and the empty-results box.
- **Hero Gradient** (`#111827` → `#312e81`): the hero band only. Never reused elsewhere.

### Named Rules
**The Two-Accent Rule.** Only indigo and teal ever carry meaning on screen. Indigo means focus or selection; teal means status or count. Amber exists solely to mark a search hit. Introducing a third "meaningful" hue anywhere else is a bug, not a design choice.

## 3. Typography

**Display / Body / Label Font:** Inter (with `ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif` fallback)

**Character:** One geometric-humanist sans doing every job — hierarchy comes from scale and negative tracking, not from switching families or leaning on italics/weight extremes.

### Hierarchy
- **Display** (700, `clamp(28px, 3vw, 44px)`, line-height 1.15, tracking -0.04em): the hero `<h1>` only.
- **Headline** (700, 28px, line-height 1.2, tracking -0.04em): the term detail title once a term is selected — the largest heading a user sees mid-task.
- **Title** (700, 24px, line-height 1.25, tracking -0.035em): the branch/section title above the term grid.
- **Body** (400, 14px, line-height 1.5): detail-panel paragraphs and card subtitles; card subtitles run slightly smaller at 13px. Cap prose at ~70ch even though panels are narrow enough that this rarely binds.
- **Label** (600, 12px, line-height 1.35, tracking 0.08em, uppercase): section labels inside the detail panel ("Что означает", "Зачем UX-исследователю"). The smallest chips (tags, badges) drop to 11px at the same weight/tracking family.

### Named Rules
**The One-Family Rule.** Inter carries every role from hero to label. A second typeface — for "warmth," for a serif accent, for anything — does not enter this system without a deliberate typeset pass.

## 4. Elevation

Flat by default. Panels get exactly one ambient shadow token; nothing escalates that shadow on interaction. Selection and hover are communicated through a focus ring and a 1px translateY lift, never through a heavier shadow.

### Shadow Vocabulary
- **Ambient Panel** (`box-shadow: 0 12px 34px rgba(15,23,42,.08)`): the hero band and every `.panel` (nav, content, detail). The only "resting" shadow in the system.
- **Card Hover** (`box-shadow: 0 10px 20px rgba(15,23,42,.07)`, paired with `transform: translateY(-1px)`): term cards only, on hover.
- **Focus Ring** (`box-shadow: 0 0 0 4px rgba(79,70,229,.12)`): the active term card and any focused input/select. This is a ring, not a shadow — it signals state, not depth.

### Named Rules
**The Ring-Not-Shadow Rule.** Selection state is a 4px indigo ring, never a darker or larger shadow. Shadows stay reserved for ambient panel elevation and the one hover-lift on term cards.

## 5. Components

### Buttons
- **Shape:** 14px radius (`rounded.sm`).
- **Primary:** solid Indigo Focus fill, white text, 12px/14px padding, no border. No hover/active treatment is currently defined — a gap worth closing before this button ships on a new surface.

### Chips / Pills / Badges
- **Style:** 999px radius on every instance — the pill shape is exclusive to status and meta chips (counter, mode pill, cluster badge, tags, related-term chips) and must never appear on anything else.
- **Status pill:** Teal Status text on Teal Status Bg with a matching-hue border (mode pill).
- **Badge:** Indigo Deep text on white with a light indigo border (cluster badge, detail cluster tag).
- **Neutral tag/chip:** Tag Text or Body Text on Surface Soft or Surface, hairline Border — used for cluster labels on cards and for related-term chips, which additionally invert to Indigo Focus text/border on hover.

### Cards / Containers
- **Corner Style:** 18px radius on term cards, 22px on panels, 28px on the hero (22px at the ≤820px breakpoint).
- **Background:** Surface (white) on Neutral Bg.
- **Shadow Strategy:** see Elevation — ambient shadow on panels, hover-lift + focus-ring on cards, nothing on the hero besides the ambient shadow.
- **Border:** 1px hairline Border by default; Border Strong on hover.
- **Internal Padding:** 14px cards, 18-20px panel interiors, 14px nav panel.

### Inputs / Fields
- **Style:** white background, 1px hairline border, 14px radius, 12px/14px padding.
- **Focus:** border shifts to Indigo Focus plus a 4px indigo glow ring (`0 0 0 4px rgba(79,70,229,.12)`) — the same ring language as card selection.

### Navigation
- **Style:** the left branch-nav panel is a vertical list of full-width, left-aligned buttons (16px radius, 12px padding). Inactive is transparent-on-hover-to-Surface-Soft; active gets an Indigo Weak background with a light indigo border. Each item pairs a bold branch name with a muted description line and an item-count badge, so the nav itself teaches the taxonomy before a single term is opened. On mobile (≤1180px) it stops being sticky and stacks above the content.

### Detail Panel (signature component)
- Sticky right-hand panel, scoped by a cluster pill, a headline-level term title, then stacked labeled blocks ("Что означает" / "Зачем UX-исследователю" / "Связанные понятия") separated by hairline top-borders. Related concepts render as a wrapped row of pill chips that re-trigger selection on click — this is the mechanism that turns a flat glossary into a mind-map, and any redesign should preserve the label → block → related-chips rhythm rather than collapsing it into a single paragraph.

## 6. Do's and Don'ts

### Do:
- **Do** keep the pill shape (999px) exclusive to status/meta chips — counter, mode pill, badge, tag, related chip. Nothing else gets rounded past 22px.
- **Do** use the 4px indigo focus ring for every selection/focus state (inputs, active cards) instead of inventing a new selection treatment per component.
- **Do** pair Indigo Focus with white text and Teal Status with its own tinted background — never cross the two accents' color-on-color pairings.
- **Do** keep hover motion to the existing vocabulary: 1px lift + soft shadow on cards, border-color shift on chips. Nothing heavier.
- **Do** treat the term-card grid as the one earned exception to "cards are the default answer" — it exists because the content is genuinely a set of parallel browsable items.

### Don't:
- **Don't** add gradient text anywhere, including the hero headline — emphasis comes from size and weight, never `background-clip: text`.
- **Don't** drift the background toward a cream/sand near-white "for warmth." PRODUCT.md explicitly names that as the generic-AI-SaaS tell to avoid; if warmth is needed, it comes from copy, illustration, or a deliberately chosen accent — not a beige body background.
- **Don't** introduce a third "meaningful" accent hue. Indigo = focus, teal = status. A new color needs a new rule, not a one-off usage.
- **Don't** add tiny uppercase tracked eyebrows or numbered section markers (01 / 02 / 03) as default scaffolding — none exist today and none should be added reflexively.
- **Don't** mistake this document for permission to ship new team-facing surfaces as-is. PRODUCT.md's target personality is "warm & approachable"; this indigo/slate baseline is calm and precise, not warm. Run `/impeccable colorize` or a deliberate redesign pass on any new surface where that gap matters, rather than copying this palette forward by default.
