---
version: "alpha-2.1"
name: "Space-Age Archive Console"
description: "Agent-curated design language. Mid-to-late 1960s Space Age industrial design — DEC minicomputer front panels and Apollo program consoles — encountered fifty years later, in ambient light, unpowered. Warm aged palette, hard color seams, stenciled hierarchy. No neon, no glow. Named component library, drill-down expansion pattern, interactive states, derived state tints, two-mode density system. v2.1 adds the comment-thread pattern for review discussions, an inline-code-in-prose rule for technical writing, and clarified case discipline (all-caps applies to UI chrome, not to data content)."
colors:
  primary: "#604041"
  secondary: "#7E635F"
  accent: "#D34B46"
  background: "#1F1C1A"
  surface: "#2F2E2D"
  text: "#E6D2BE"
  muted: "#AF988F"
  border: "#3A312E"
  error: "#D34B46"
  success: "#6F8A6F"
  warning: "#E48282"
  info: "#7E635F"
derived-colors:
  hover-tint: "rgba(96, 64, 65, 0.08)"
  active-tint: "rgba(96, 64, 65, 0.10)"
  switch-off-bg: "#9C6868"
  pink-text: "#5A2828"
  pink-text-muted: "#4A2A2A"
typography:
  headline-lg:
    fontFamily: "Jost"
    fontSize: "1.953rem"
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  headline-md:
    fontFamily: "Jost"
    fontSize: "1.563rem"
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: "-0.01em"
  body-md:
    fontFamily: "Inter"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "0"
  label-md:
    fontFamily: "IBM Plex Mono"
    fontSize: "0.75rem"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.08em"
  code-inline:
    fontFamily: "IBM Plex Mono"
    fontSize: "0.9em"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "0"
rounded:
  none: "0px"
  sm: "0px"
  md: "0px"
  lg: "2px"
  full: "9999px"
spacing:
  base: "8px"
  xs: "4px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "24px"
  2xl: "32px"
  3xl: "48px"
  4xl: "64px"
  step-8: "96px"
density-modes:
  archive:
    module-padding: "22px"
    row-padding: "14px"
    grid-gap: "24px"
    masthead-padding-y: "20px"
  operational:
    module-padding: "18px"
    row-padding: "8px"
    grid-gap: "20px"
    masthead-padding-y: "12px"
components:
  color-reference-primary:
    backgroundColor: "{colors.primary}"
  color-reference-secondary:
    backgroundColor: "{colors.secondary}"
  color-reference-accent:
    backgroundColor: "{colors.accent}"
  color-reference-background:
    backgroundColor: "{colors.background}"
  color-reference-surface:
    backgroundColor: "{colors.surface}"
  color-reference-text:
    backgroundColor: "{colors.text}"
  color-reference-muted:
    backgroundColor: "{colors.muted}"
  color-reference-border:
    backgroundColor: "{colors.border}"
  color-reference-error:
    backgroundColor: "{colors.error}"
  color-reference-success:
    backgroundColor: "{colors.success}"
  color-reference-warning:
    backgroundColor: "{colors.warning}"
  color-reference-info:
    backgroundColor: "{colors.info}"
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.text}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
  card-surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.text}"
    rounded: "{rounded.none}"
    padding: "{spacing.lg}"
  input-default:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.text}"
    rounded: "{rounded.none}"
    height: "44px"
  indicator-pip:
    backgroundColor: "{colors.text}"
    rounded: "{rounded.full}"
    width: "7px"
    height: "7px"
  switch-cap:
    backgroundColor: "{colors.warning}"
    textColor: "{derived-colors.pink-text}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
  drilldown-panel:
    backgroundColor: "{colors.background}"
    textColor: "{colors.text}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
  code-inline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.text}"
    typography: "{typography.code-inline}"
    rounded: "{rounded.none}"
    padding: "1px 5px"
---

# Space-Age Archive Console

## Overview

Space-Age Archive Console is a contemplative interface language built from the visual grammar of mid-to-late 1960s Space Age engineering — Apollo guidance consoles, DEC PDP minicomputer front panels, the silkscreened control modules of Mission Control — encountered fifty years later. Everything is still legible, still beautifully engineered, but the room is quiet and the equipment is unpowered. Burgundy and mauve-brown bands stand in for the bright magenta of the original hardware; charcoal enamel replaces glossy black; warm ivory labels read clearly against panels softened by decades. A single DEC-red accent stripe survives unfaded. Pink switch caps wait under their plastic covers to be flipped, but nothing glows. The language is for interfaces that want the discipline and warmth of mid-century industrial design without nostalgia kitsch, without neon, and without pretending the equipment is new.

### Values

- Aged industrial calm: every surface looks like enameled steel or yellowed ABS plastic, never glass or glow. Decoration belongs to the equipment, not to the moment of viewing.
- Banded mastheads and labeled modules: each major region behaves like a fabricated console — a burgundy or mauve-brown horizontal band carries a lowercase section title; a charcoal panel face holds the controls and readouts beneath.
- Stenciled hierarchy: the eye moves from lowercase friendly headers to ALL-CAPS regulatory labels to outlined highlight terms. Warm ivory text carries most informational weight; weight itself is never a hierarchy tool.
- Octal-triple grouping where content cooperates: rows of three feel native; rows of four feel imposed. Where the content forms natural triples (HTTP status classes, telemetry pipelines, sensor groups), embrace the grouping. Don't force it where it resists.
- One accent color, used sparingly in chrome: DEC-red appears at most twice in screen chrome — a masthead stripe, a primary action, an error chip. Hairline structural marks at 1–2px (drilldown indicators, focus rings) don't count against the chrome quota.
- Quiet typography: lowercase Jost (or equivalent geometric sans, Futura Demi family) for friendly headers, ALL CAPS Inter (or Helvetica family) for institutional labels, IBM Plex Mono for telemetry and code. Always regular weight; case and color carry hierarchy.

### Anti-Values

- Neon highlighting, glowing accents, luminous text, or any simulation of emission. The equipment is photographed in ambient light, not powered up.
- Drop shadows, soft shadows with blur radius > 0, glassmorphism, neumorphism, or any floating-surface treatment. Surfaces are inlaid into the panel, never hovering above it. (1px hard outlines for focus or framing are not shadows.)
- Bold weight as a hierarchy tool. Hierarchy comes from case, color band, and outline treatment.
- Brand-bright magenta, candy pastels, sky-blues, or any color choice that erases the aged warmth. The world is warm and slightly faded.
- Decorative emoji or illustrated iconography. Semantic icons are stenciled geometric pictograms (triangle, circle, square, hairline arrow). State indicators (toggle, count) may use mono-cap typography.
- Animation beyond instant state swap. No fade-in, no slide-down, no easing on expand. State changes are mechanical: before and after, no between.
- Syntax highlighting on code. The warm palette has no place for the conventional purples, blues, and bright greens of editor themes. Code is monochrome; if changes need to be marked (diff view), use the restrained sage/pink diff tint scheme.

### Visual Character

- Charcoal enamel panel ground (#2F2E2D) seated inside a deep-shadow ambient field (#1F1C1A), separated by a 1px warm-brown seam.
- Burgundy (#604041) and mauve-brown (#7E635F) full-width horizontal bands serve as section mastheads, each carrying a lowercase friendly title in warm ivory.
- White stencil-outline highlight: emphasized terms render with `color: transparent` and a 1px ivory text-stroke, letting the underlying panel color show through letter interiors — like engraved aluminum signage from a NASA bulkhead plate.
- Pink switch caps (#E48282) used as rectangular toggle elements, grouped in threes; the off state desaturates to #9C6868 and loses its ivory outline border.
- Matte ivory indicator pips (4–8px squares or circles), never glowing; "on" is a filled ivory shape, "off" is the same shape filled with mauve-brown.
- DEC-red accent (#D34B46) appears once or twice per screen as chrome — a 3px horizontal rule beneath a masthead, the background of a single primary action, or the border of an error condition. Hairline structural use at 1–2px (drilldown markers, focus stripes) is unrestricted.
- Telemetry and register displays in IBM Plex Mono caps, ivory on charcoal, framed by 1px warm-brown rules above and below to evoke the Apollo DSKY.
- Drill-down expansions render inline beneath the trigger row, in a slightly darker background, with a 2px hairline accent or ivory marker on the left edge.
- Discussion threads (comments, annotations) render as stacked cards with 1px left-border accents — the border color distinguishes content authors (ivory) from reviewers (border) without color-coding by individual.

## Colors

Use the YAML color tokens as the normative palette. The prose below names the roles agents should preserve when generating UI.

| Token | Value | Role |
|-------|-------|------|
| primary | `#604041` | Deep plum / burgundy. Section masthead bands, primary chrome, authoritative surfaces. The aged form of the original aubergine. |
| secondary | `#7E635F` | Dusty mauve-brown. Secondary masthead bands, alternating row labels, quieter section identity. |
| accent | `#D34B46` | DEC red stripe. The single unfaded color. Reserved for masthead rules, primary action backgrounds, error states — and for hairline structural marks. |
| background | `#1F1C1A` | Deep near-black shadow. The ambient room around the panels — gutters, page edges, dim negative space, drilldown panel ground, inline-code surface. |
| surface | `#2F2E2D` | Charcoal enameled panel. The fabricated module faces where controls and content live. |
| text | `#E6D2BE` | Warm ivory / silkscreened label color. The primary readable color on every panel. |
| muted | `#AF988F` | Warm beige plastic aging. De-emphasized labels, off-state indicator fills, weathered decals, dashed reference lines. |
| border | `#3A312E` | Panel seam. Hard 1px lines between charcoal panels and deep-shadow gutters. |
| error | `#D34B46` | Shares value with accent. Error states are critical attention; they earn the rare bright color. |
| success | `#6F8A6F` | Faded sage / aged "GO" indicator. The single permitted concession outside the warm palette — a desaturated Mission Control go-flag green. Use sparingly. |
| warning | `#E48282` | Pink switch cap. Soft warning that retains the equipment's signature color. Used for pink switches, warning event marks, slow trace spans. |
| info | `#7E635F` | Shares with secondary. Quiet informational annotations live in the secondary band color. |

### Derived State Tints

For interaction states and contrast pairings, use these derived values rather than inventing new ones. Each derives from a token in the canonical palette and stays in the warm-aged family.

| Token | Value | Use |
|-------|-------|-----|
| hover-tint | `rgba(96, 64, 65, 0.08)` | Background overlay on interactive rows on hover. Primary at 8% opacity, sits on top of `surface`. |
| active-tint | `rgba(96, 64, 65, 0.10)` | Background overlay on open / selected rows. Primary at 10% opacity. Slightly darker than hover so state is distinguishable. |
| switch-off-bg | `#9C6868` | Desaturated warning for the off-state pink switch cap. Approximately warning at 70% saturation. |
| pink-text | `#5A2828` | Dark plum text on any pink surface (warning or switch-off-bg). Needed for legibility; pure ivory on pink fails contrast. |
| pink-text-muted | `#4A2A2A` | Slightly darker variant for off-state switch caps where the overall surface is duller. |

## Typography

- **Headline-Lg**: Jost, 1.953rem (~31px), weight 400, line-height 1.2, letter-spacing -0.01em. **Set in lowercase.** This is the friendly section header that names each console module.
- **Headline-Md**: Jost, 1.563rem (~25px), weight 400, line-height 1.25, letter-spacing -0.01em. **Set in lowercase.** Subsection headers.
- **Body-Md**: Inter, 16px, weight 400, line-height 1.55, letter-spacing 0. Long-form reading and explanatory paragraphs.
- **Label-Md**: IBM Plex Mono, 0.75rem (~12px), weight 500, line-height 1.2, letter-spacing 0.08em. **Set in ALL CAPS.** Used for institutional labels, telemetry register names, timestamps.
- **Code-Inline**: IBM Plex Mono, 0.9em (relative to surrounding text), weight 400, line-height 1.4, letter-spacing 0. **Native case preserved.** Used for inline code references within body prose.

### Display Caps (Core Important Text)

Core important text is set in **regular-weight, ALL CAPS warm ivory**, never bold. Use either the Inter or Jost family at body or label sizes, with letter-spacing 0.10em to 0.12em. This is how regulatory labels — VERB, NOUN, STATUS, EXEC, SEQUENCE, ABORT — appear throughout the panel. The text reads as silkscreened or engraved onto the equipment, and weight is intentionally restrained so that the all-caps treatment alone carries the emphasis.

### Case Discipline

The all-caps treatment applies to **UI chrome** — labels, statuses, metadata, regulatory text on the panel itself. It does **not** apply to **data content** displayed on the panel: code, multi-case identifiers, file paths with case sensitivity, user-generated text, prose passages, mixed-case product names. These render in their native case using the appropriate face (`code-inline` or mono for code and identifiers, `body-md` for prose, `label-md` only when the content really is institutional labeling).

The discipline is about how the equipment *speaks*, not about what it *displays*. A serial number on a panel decal is ALL CAPS because it's part of the equipment; a Go function name displayed in a diff is `mixedCase` because it's the content being inspected. The equipment doesn't transform its content; it presents it accurately.

### Stencil Outline Highlight

For singular emphasized terms, apply the stencil outline treatment:

```css
.highlight {
  color: transparent;
  -webkit-text-stroke: 1px var(--text);
  text-stroke: 1px var(--text);
}
```

This produces text whose letter interiors show the underlying panel color — an engraved-aluminum effect borrowed directly from Apollo-era equipment signage.

**When to use:** singular state markers (the one active nav item, a session identifier, a current selection); single emphasized terms in a paragraph (one word, not three). Reserve for ≥16px text where the stroke remains legible.

**When not to use:** multiple terms in close proximity, long passages, small labels (<14px), or anywhere readability of the content matters more than the typographic gesture.

### Inline Code in Prose

Inline `<code>` elements within body-md prose use the mono family at 0.9em (relative to the surrounding text), set on the `background` color (one shade darker than the surrounding `surface`), with a 1px `border` outline and 1–5px horizontal padding. The text color stays `text` — never colored, never highlighted.

```css
.body-prose code {
  font-family: var(--font-mono);
  font-size: 0.9em;
  background: var(--background);
  border: 1px solid var(--border);
  padding: 1px 5px;
  color: var(--text);
  border-radius: 0;
}
```

The result reads as a small inset window onto a technical referent — a brief surface change inside the prose, consistent with how the language treats data elsewhere on the panel (deeper background, hard 1px border, no fill color). Native case is preserved per Case Discipline above.

Block code (multi-line) follows the same color rules and may add the restrained diff-tint treatment when displaying changes: sage tint (`rgba(111, 138, 111, 0.10)`) for added lines, pink tint (`rgba(228, 130, 130, 0.08)`) for removed lines, both with mono prefix glyphs (`+` in success, `−` in warning). Standard editor syntax highlighting is forbidden.

### Family Substitutions

Jost is the closest free Google Fonts equivalent to Futura Demi; substitute Futura, Avenir, or Twentieth Century where licensing permits. Inter is the closest free equivalent to Helvetica Neue; substitute Helvetica, Neue Haas Grotesk, or Pragmatica where licensing permits. IBM Plex Mono is the canonical telemetry and code face; substitute JetBrains Mono or Berkeley Mono where preferred.

Google Fonts URL:
```
https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Jost:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500;600&display=swap
```

## Layout

### Spacing Tokens

- **Base**: `8px`
- **Xs**: `4px`
- **Sm**: `8px`
- **Md**: `12px`
- **Lg**: `16px`
- **Xl**: `24px`
- **2xl**: `32px`
- **3xl**: `48px`
- **4xl**: `64px`
- **Step-8**: `96px`

### Density Modes

The language has two density modes, both built from the same tokens and patterns but tuned for different attention rhythms.

**Archive mode** is the calmer end — long-attention review work, historical browsing, single-event inspection. Modules breathe. Ground-station and observation-log scenarios live here. Use when the screen will be read slowly by one person at a time.

- Module body padding: `22px`
- Row padding: `14px`
- Grid gap: `24px`
- Masthead vertical padding: `20px`

**Operational mode** is the denser end — service monitoring, post-incident review, multi-metric dashboards, code review. Information packs without losing the hard-seamed, labeled character. Observability and review-workflow scenarios live here. Use when the screen needs to surface many data points or facets in one view.

- Module body padding: `18px`
- Row padding: `8px`
- Grid gap: `20px`
- Masthead vertical padding: `12px`

The same tokens, the same patterns, the same chrome — only the rhythm changes. A single product may use both modes on different screens (an archive landing page vs. an active monitoring dashboard).

### Grid

The 9-column grid is the default and the flavor choice — three "octal groups" of three columns each, with 24px gutters at max-width 1320px. It embeds triple-grouping into the layout bones and is preferred where content forms natural triples.

A 12-column grid is acceptable where layout demands it (heavy mixed-width modules, content that doesn't divide into thirds). What matters is the discipline of grid-snapping and the rhythm of three within content, not the column count itself.

Tablet collapses to 6 columns at 900px. Mobile becomes a single column of stacked modules, each retaining its full masthead band.

### Breakpoints

Use responsive cuts at 1180px, 900px, 768px, and 480px. At 900px multi-column grids collapse to 6. At 768px masthead bands compress and lowercase headers wrap to a second line if necessary. At 480px tables become horizontal scroll, KPI grids stack vertically, and pink switch groups stack.

### Whitespace

Whitespace is the deep-shadow gutter between panel modules — it should feel like the dark spaces between consoles in a Mission Control room, not like inviting page margin. Keep gutters generous (20–48px depending on density mode) and resist filling them with decoration; the emptiness is part of the language.

### Responsive

- **Desktop**: 1440px 9-column octal grid with three-by-three module layout
- **Tablet**: 768px two-octal grid with right group stacked below
- **Mobile**: 375px single-column panel stack with full-width masthead bands

## Elevation & Depth

### Shadows

- **Sm**: `inset 0 1px 0 rgba(0,0,0,0.4)` — slight inset to suggest the panel surface is recessed into a frame.
- **Md**: `inset 0 2px 0 rgba(0,0,0,0.5)` — pressed / depressed state for active switches and buttons.
- **Lg**: `0 0 0 1px #3A312E` — 1px hard outline used as a focus ring or framing rule. Not a soft drop shadow.

No drop shadows. No glows. No halo effects. No `box-shadow` with `blur-radius > 0`. All depth comes from inset depression or 1px hard outlines.

### Focus and Hover

Interactive elements need state feedback, but the language forbids glow. Use these instead:

- **Hover** on rows, table cells, and clickable list items: apply `hover-tint` (`rgba(96, 64, 65, 0.08)`) as a background overlay. Instant, no transition. Hover on a button or switch additionally deepens its inset shadow.
- **Focus** on inputs, buttons, and switches: 1px hard ivory outline (`outline: 1px solid var(--text)`), no offset, no glow, no transition. For the focused element to stand out against pink switch caps, the ivory outline reads through.
- **Active / Open / Selected** state: apply `active-tint` (`rgba(96, 64, 65, 0.10)`) as a background overlay — slightly darker than hover so the difference is readable.
- **Pressed / Depressed**: deepen the inset shadow to `inset 0 2px 0 rgba(0,0,0,0.5)`. Buttons and switches feel like they've been pushed into the panel.

All state changes are instant. No fades, no eases, no transitions on color or background.

## Shapes

### Rounded

- **None**: `0px`
- **Sm**: `0px`
- **Md**: `0px`
- **Lg**: `2px`
- **Full**: `9999px` — reserved exclusively for round indicator pips and the rare circular status mark.

The original equipment was rigidly rectangular. Default to 0px on every container, button, field, and band. Use 2px only when a small softening genuinely serves the design; use full only on indicator pips.

### Surfaces

- **Treatment**: enameled steel panel with aged ABS plastic accents
- **Card Style**: Charcoal enamel modules separated by deep-shadow gutters. Each module has a burgundy or mauve-brown masthead band at its top carrying a lowercase friendly title in warm ivory. Internal content sits directly on the charcoal — no inner card-within-card nesting except for drill-down expansion panels, which use the deep-shadow background.
- **Bg Pattern**: subtle matte grain. Barely visible noise suggesting painted steel rather than glass or paper.

### Borders

- **Default Width**: 1px
- **Accent Width**: 3px (chrome) / 2px (structural)
- **Style**: solid
- **Character**: Hard color seams between panel bands. Warm-brown 1px seams (`#3A312E`) between charcoal modules and deep-shadow gutter. DEC-red 3px stripes as chrome rules beneath masthead bands. DEC-red 2px hairline as structural drilldown markers and focus stripes. Never anti-aliased softness; never dashed (except dotted reference lines on chart axes); never animated.

## Components

### Composition

Treat each screen as a fabricated console set inside a quiet room. The outer frame is deep shadow; content sits on charcoal enamel panels divided by horizontal burgundy and mauve-brown bands. Mastheads are full-width banded sections with a lowercase friendly header in warm ivory and an optional ALL-CAPS aux annotation on the right (status, count, instruction). Beneath each masthead, controls, readouts, and indicator pips cluster in groups of three when possible. Asymmetry is acceptable, even encouraged, but everything snaps to the grid. The page should feel like equipment, not like a webpage — like a museum diorama of the future as imagined in 1969, with new instruments installed in the original frame.

### Hierarchy

Lowercase friendly headers (Jost, regular weight, warm ivory) name each module and live inside the masthead band. ALL-CAPS Helvetica-family text in regular-weight warm ivory carries regulatory or institutional labels at body or label size. Outlined stencil text highlights singular emphasized terms by letting the panel show through letter interiors. IBM Plex Mono caps carries telemetry, numeric registers, timestamps, sequence codes, and any tabular reading. Mixed-case IBM Plex Mono carries code, identifiers, and file paths displayed as data content (see Case Discipline in Typography). Bold weight is forbidden as a hierarchy tool; case, color band, and outline treatment do the work.

### Density

Medium in archive mode, dense in operational mode (see Layout § Density Modes). Both modes share the same hierarchy, the same color discipline, and the same component vocabulary; only the rhythm changes.

### Component Library

Twelve named components form the working vocabulary. Each is small. Together they cover most of what a console-style product needs.

- **meta-block**. A caps-label-over-caps-value pair stacked in a column, used in mastheads, registers, and controls-meta blocks. Label is `caps-label` (0.625rem, opacity 0.68); value is `caps-value` (0.8125rem, full opacity). Two lines, tight gap.

- **module-masthead**. A full-width banded header inside a module, padded 10–12px. Carries the lowercase friendly title on the left and an optional ALL-CAPS aux annotation on the right (status, count, instruction like "CLICK ROW TO INSPECT"). Background is `primary` or `secondary` depending on visual rhythm; alternate to avoid two adjacent same-colored bands.

- **kpi-cell**. A label/value/state stack used in vitals grids (typically 2×3 or 3×2). Top: `caps-label`. Middle: large mono value with optional small mono unit. Bottom: `caps-label`-sized state pill, colored by token (`success` for nominal, `warning` for elevated/degraded).

- **register-row**. A 3-column grid: NOUN-name (mono caps, muted), value (mono, right-aligned), unit-label (mono caps, muted, left-aligned in a fixed-width column). Maps directly to the Apollo DSKY readout. Use for any sequence of named numeric or short-text values.

- **switch-cap**. A pink rectangular toggle (or radio member). On state: warning background, dark-plum text, 2px ivory outline inset 5px. Off state: switch-off-bg background, pink-text-muted text, no outline. Deepened inset shadow when pressed. Always grouped — single switches feel orphaned.

- **indicator-pip**. A 4–8px round or square pip. On state: ivory fill. Off state: secondary fill, optional 1px border. Warning state: pink fill. Optionally paired with a caps-label to its right. Never glows.

- **drilldown-panel**. An inline expansion below a trigger row. Distinct from the parent module surface by sitting on `background` (one shade darker than `surface`), with a 2px hairline accent-color left border. Internal padding 14×18px. Internal layout is a 130px / 1fr key-value grid for short attributes, or section-titled blocks for richer content. See Drill-down Expansion below for the full specification.

- **mini-bar**. A 6px-tall horizontal segmented bar, used inline for distributions (status code splits, traffic share, etc.). Segments use `muted`, `warning` (low opacity), and `warning` (full) for an ok/warn/error tristate. Background between segments is `border`.

- **slo-bar**. A longer 10px-tall track with fill. Track background is `background` with a 1px `border` outline. Fill is `text` (healthy) or `warning` (depleted/endangered). Accompanied above by name+target meta-block and below by a percentage value (`text` or `warning`).

- **method-badge**. A small bordered caps rectangle (POST, GET, PUT). 1px `border` border, mono caps, padding 3×6px. Write methods optionally use a secondary border for visual weight; reads as a stamped label, not a colored pill.

- **attribute-list**. An inline `key=value · key=value · key=value` pattern for compact attribute display. Keys in muted, the `=` separator in secondary, values in text. Used heavily inside drilldown panels and anywhere structured metadata needs to fit in flowing space.

- **comment-thread**. A discussion pattern for review comments, annotations, and other back-and-forth threaded text. Composed of a context header (file path or referent location in mono caps muted, plus a state indicator `RESOLVED` / `UNRESOLVED` in caps with a 1px border colored by `muted`/`success`/`warning`), followed by one or more comment cards. Each card carries a 1px left border — `border` color for reviewer comments, `text` (ivory) color for the content author's own comments. The author-distinction is structural, not chromatic — no author badges, no fills, just the border weight and color making the speaker obvious. Card content: a header row with author name (mono caps), optional author tag (e.g., `AUTHOR`), timestamp (mono caps muted), and decision state (`APPROVED` / `CHANGES REQUESTED` in `success`/`warning`); a body in body-md prose that may contain inline-code per the typography rule. Threads may include a **diff-line-comment-anchor** in the source view — a single inline row (`◇ 02 COMMENTS · LINE 33`) between diff lines, in `warning` mono caps, indicating that a thread anchors to this line. The anchor is a pointer; the thread itself renders in a discussion module elsewhere on the page.

### Drill-down Expansion

Drill-downs let users expand a row to inspect its full content without leaving the page. The pattern:

- **Trigger**: any clickable row in a list, table, or trace. Includes a `+` indicator on the right (instant swap to `−` when open). Hover state applies `hover-tint`; open state applies `active-tint`.
- **Mechanism**: inline insertion of an expansion panel immediately below the trigger row. No modal, no popover, no slide-out. The page reflows; everything below shifts down by the panel height. Instant — no transition.
- **Container**: `drilldown-panel` component. Background `background` (one shade darker than parent `surface`), padding 14×18px, 2px `accent` left border to mark depth-of-attention. Indented matching the parent module body padding so the panel reads as a child, not a sibling.
- **Internal layout**:
  - Short attributes: 130px label / 1fr value grid, mono caps keys in muted, mono values in text.
  - Sections of attributes: `drilldown-section-title` (mono caps, very small, muted, with 1px border-bottom rule).
  - Free-form inline metadata: `attribute-list` (`key=value · key=value`).
  - Sub-event rows: 110px time / 1fr description grid, similar density to the parent row.
  - Cross-links: `drilldown-link` — mono, ivory, with 1px dashed underline that becomes solid on hover.
- **Multi-open**: multiple drill-downs may be open simultaneously. The state is per-row, not exclusive.
- **Auto-open**: prefer auto-opening the most relevant row on initial render (the slowest trace span, the highest-priority alert, the top-volume endpoint, the most-discussed comment thread). It demonstrates the affordance without requiring discovery.

### Interactive States

| State | Treatment |
|-------|-----------|
| Default | Token colors, no overlay. |
| Hover | `hover-tint` background overlay. Instant. Cursor: pointer for clickable. |
| Active / Open / Selected | `active-tint` background overlay. Instant. |
| Focus | 1px hard ivory outline, no offset, no glow. |
| Pressed | Deepened inset shadow `inset 0 2px 0 rgba(0,0,0,0.5)`. |
| Disabled | Reduced opacity 0.45, no hover response, no focus. Avoid where possible — prefer to hide controls that don't apply. |

No transitions on any state property. Hover, focus, and active are instantaneous.

### Pictograms and Glyphs

The language distinguishes two kinds of small marks:

- **Pictograms** are semantic icons — meanings, not data. Use stenciled geometric forms only: triangle (warning), circle (status/on), square (stop), hairline arrow (sequence/navigation), diamond (annotation anchor). Drawn as 1px ivory strokes, never filled, never colored beyond accent or warning.
- **Glyphs** are state indicators or compact data — counts, toggles, sorts. Use mono-cap typography rather than pictograms: `+` and `−` for expand/collapse, `▲` and `▼` for sort order, `◀` for selection-pointer, numeric counts in mono. Glyphs are typography, not iconography, and follow the type rules (regular weight, all-caps where the surrounding context is all-caps).

This resolves the apparent contradiction between "no decorative iconography" and the need for state indicators. Pictograms communicate meaning; glyphs communicate state.

### Signature Patterns

- Lowercase friendly section headers in geometric sans (Jost, Futura Demi family), regular weight, warm ivory, set directly inside a burgundy or mauve-brown masthead band that runs the full width of the module. Optional ALL-CAPS aux annotation on the right.
- White stencil outline on emphasized text: `color: transparent; -webkit-text-stroke: 1px #E6D2BE;` creates an engraved-aluminum effect where the underlying panel shows through letter interiors. Reserve for singular state markers and single emphasized terms at ≥16px.
- ALL-CAPS regulatory labels in regular weight (never bold), tracked +0.08em to +0.12em, in warm ivory. These read as silkscreened directly onto the panel. Applied only to UI chrome — never to data content (see Case Discipline).
- Pink switch caps (#E48282) rendered as rectangular toggle elements, grouped in threes wherever content allows. Off state desaturates to switch-off-bg and loses its ivory outline border.
- Matte ivory indicator pips (4–8px), square or circle, ivory fill = on, mauve-brown fill = off, warning fill for attention. No glow under any condition. No animation on state change beyond an instant swap.
- DEC-red accent as chrome (3px masthead stripe, primary action background, error chip border) — at most twice per screen. DEC-red as structural hairline (drilldown left edge, focus stripe) at 1–2px width — unrestricted.
- Telemetry and register displays in IBM Plex Mono caps, ivory on charcoal, framed by 1px warm-brown rules above and below — directly evocative of the Apollo DSKY register display.
- Drill-down panels indented from the parent module body, on `background`, with a 2px hairline accent-color left edge. Internal key-value grid or section-titled blocks. Instant expand and collapse.
- Mini-bars for inline distributions; SLO bars for longer single-metric burndowns. Both use the same warm palette (muted / warning) and live within otherwise typographic surrounds.
- Method badges as small 1px-bordered caps rectangles, never colored fills. They behave like silkscreened stamps on the equipment.
- Comment threads render with each comment card carrying a 1px left border — `border` for reviewer comments, `text` (ivory) for content author comments. Author distinction is structural, not chromatic. Inline-code references within comment bodies follow the typography rule (mono, `background` fill, 1px `border`).
- Inline code in body prose appears as a small inset window — mono family at 0.9em, on `background`, with a 1px `border` outline. Never highlighted, never colored. Block code may use the restrained diff-tint scheme (sage / pink) when displaying changes.
- Stenciled geometric pictograms (1px ivory strokes) for semantic icons; mono-cap glyphs for state indicators.

## Do's and Don'ts

### Do

- Set section titles in lowercase Jost (or equivalent geometric sans), regular weight, warm ivory, inside a burgundy or mauve-brown masthead band.
- Use ALL CAPS warm-ivory text in regular weight for institutional / regulatory labels: VERB, NOUN, STATUS, EXEC, SEQUENCE, ABORT.
- Apply the all-caps rule to UI chrome (labels, statuses, metadata, regulatory text). Render code, identifiers, file paths, and long-form prose in their native case using the appropriate face.
- Apply the white-outline-on-background stencil treatment to singular emphasized terms at ≥16px (active state, key identifier, current selection).
- Group controls and indicators in threes when content allows. Where it doesn't, prefer 6 or 9 (multiples of 3) before 4 or 8.
- Use DEC-red as chrome at most twice per screen (masthead stripe, primary action, error chip). Use DEC-red as 1–2px hairline structural marks (drilldown indicator, focus stripe) freely.
- Render telemetry, register values, timestamps, and sequence codes in IBM Plex Mono caps, ivory on charcoal, framed by 1px warm-brown rules.
- Treat indicator pips as matte: ivory fill = on, mauve-brown fill = off. Pips never glow.
- Use 0px radii on all containers, buttons, fields, and bands. Reserve `full` exclusively for round indicator pips.
- Pick a density mode (archive or operational) per screen and apply it consistently. Mixing modes within one screen reads as inconsistency, not richness.
- Use the named component library before inventing new shapes. The vocabulary covers most surfaces; reusing it is what makes the language read as a coherent system.
- Use inline code (`<code>`) on `background` with a 1px `border` and the mono family at 0.9em when referencing technical terms in body prose. Keep the text color as `text`.
- Render comment threads with the 1px-left-border author-distinction: `border` for reviewers, `text` for content authors. Use a `diff-line-comment-anchor` in the source diff to point to where each thread is rendered.
- Auto-open the most relevant drill-down on initial render to demonstrate the affordance.
- Apply derived state tints (hover-tint, active-tint) instantly with no transition.

### Don't

- Do not use neon highlighting, glowing text, luminous accents, or any emission simulation. The equipment is not powered up.
- Do not use bold weight as a hierarchy tool. Hierarchy comes from case, color band, and outline treatment.
- Do not use drop shadows, soft shadows (`blur-radius > 0`), glassmorphism, or any floating-surface treatment. Only 1px hard seams, hairline outlines, and inset depressions are permitted.
- Do not introduce greens, blues, or purples outside the established palette. The single concession is the faded sage success token — use it sparingly and pair it with a text label.
- Do not flood the screen with DEC-red chrome. More than two chrome appearances breaks the discipline. (Hairline structural use is exempt.)
- Do not round container corners beyond the established radii. The original equipment was rigidly rectangular.
- Do not use decorative emoji or illustrated iconography. Semantic icons are stenciled pictograms; state markers are mono-cap glyphs.
- Do not let any element float or simulate elevation. Surfaces are inlaid into the panel, never hovering above it.
- Do not transition any state property. No fades, no eases, no sliding panels. State changes are instant.
- Do not use the stencil outline treatment on multiple terms in close proximity, on long passages, or on small text. It is rare and singular.
- Do not apply the all-caps rule to data content. Code is not a label; file paths are not regulatory text; user-generated prose is not panel chrome. The equipment presents its content accurately.
- Do not syntax-highlight code, inline or block. The warm palette has no place for editor-theme purples, blues, and bright greens. Code is monochrome; diffs use the restrained sage/pink tint scheme only.
- Do not distinguish comment authors with colored badges, avatar tints, or text colors. The 1px-left-border distinction is sufficient and stays within the language.
- Do not invent component shapes outside the named library without good reason. The library is small on purpose; reusing it is what makes the language read as a coherent system.

### Usage Context

Best for archival viewers, museum-quality data interfaces, slow-decision dashboards, historical software emulators, telemetry replay tools, observatory and ground-station readouts, post-incident review interfaces, observability and service-health dashboards, code review and stacked-PR workflows, version control history viewers, software emulators and retro-computing tools, industrial SCADA-adjacent monitoring, and any product that wants the discipline and warmth of mid-century industrial design without nostalgia kitsch or retro-arcade glow.

Not suited for: live-action interfaces (gaming, live trading, real-time collaboration where the moment matters), consumer-playful products (kids' apps, social media, music streaming), or marketing surfaces that depend on bright energy and motion.

### Accessibility

Warm ivory (#E6D2BE) on charcoal (#2F2E2D) provides a contrast ratio of approximately 11:1 — well above WCAG AAA for body text. Warm ivory on burgundy (#604041) is approximately 8:1; on mauve-brown (#7E635F) approximately 5:1 — both above AA for large text and AAA for headlines. Verify any new text-on-color pairing maintains at least 4.5:1 for body text and 3:1 for large text.

Dark plum text (#5A2828) on warning pink (#E48282) achieves approximately 5:1 — acceptable for the short button-label use case. Avoid placing long-form text on any pink surface.

Inline code on the `background` color maintains the same 11:1 contrast as body text on `surface`, since both pair `text` against a charcoal substrate. The 1px `border` outline provides visual separation without requiring color difference.

The stencil-outline highlight treatment reduces effective contrast significantly; reserve it for emphasized terms at ≥18px where the 1px stroke remains legible. Pair the DEC-red accent, the faded sage success, and the warning pink with text labels, never relying on color alone for semantic meaning.

Maintain ≥44px tap targets on all interactive elements. Preserve visible focus outlines (1px ivory hard outline, no soft glow) on every focusable element — particularly important since the language otherwise forbids glow effects. Avoid the all-caps stencil treatment on long reading passages.

Drill-down expansions and comment threads must be keyboard-accessible: Enter or Space on the trigger row toggles open/closed; the toggle indicator must be in the page reading order; focus should remain on the trigger after expansion (not jump into the panel) unless the panel contains an interactive element that the user explicitly tabs into.
