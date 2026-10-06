---
name: Pleamar
description: Luxury villa management in Guanacaste, presented as the villa's daily conditions report.
colors:
  pacific-ink: "#0A2328"
  ink-raised: "#0F2F36"
  ink-lit: "#174450"
  on-ink: "#ECF3F1"
  on-ink-muted: "#A8C3BF"
  line-ink: "rgba(178,220,214,.17)"
  salt: "#F1F4F2"
  salt-deep: "#E2E9E6"
  paper: "#FBFCFB"
  text: "#0B2328"
  text-muted: "#435A5D"
  line: "rgba(11,35,40,.14)"
  sun-amber: "#F3AA3C"
  sun-amber-hover: "#FFBE5C"
  sun-deep: "#8F5300"
  sea-mark: "#6CCFBE"
  sea-mark-deep: "#1F8C79"
  error-line: "#FF8A7A"
  error-text: "#FFB3A8"
typography:
  display:
    fontFamily: "Antonio, Arial Narrow, sans-serif"
    fontSize: "clamp(3.3rem, 7.4vw, 6rem)"
    fontWeight: 600
    lineHeight: 0.98
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Antonio, Arial Narrow, sans-serif"
    fontSize: "clamp(2.6rem, 5.4vw, 4.75rem)"
    fontWeight: 600
    lineHeight: 1.06
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Antonio, Arial Narrow, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 600
    lineHeight: 1.05
  readout:
    fontFamily: "Antonio, Arial Narrow, sans-serif"
    fontSize: "1.75rem"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.005em"
    fontFeature: "tnum"
  body:
    fontFamily: "Hanken Grotesk, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
    fontFeature: "tnum"
  lede:
    fontFamily: "Hanken Grotesk, system-ui, sans-serif"
    fontSize: "1.1875rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Hanken Grotesk, system-ui, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.1em"
rounded:
  hair: "2px"
  sm: "3px"
  md: "4px"
spacing:
  gutter: "clamp(16px, 4vw, 56px)"
  row: "12px"
  row-loose: "16px"
  block: "56px"
  section: "clamp(88px, 11vw, 150px)"
components:
  button-primary:
    backgroundColor: "{colors.sun-amber}"
    textColor: "{colors.pacific-ink}"
    rounded: "{rounded.sm}"
    padding: "0 26px"
    height: "52px"
  button-primary-hover:
    backgroundColor: "{colors.sun-amber-hover}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-ink}"
    rounded: "{rounded.sm}"
    padding: "0 26px"
    height: "52px"
  field:
    backgroundColor: "{colors.ink-raised}"
    textColor: "{colors.on-ink}"
    rounded: "{rounded.sm}"
    padding: "12px 14px"
    height: "52px"
  field-focus:
    backgroundColor: "{colors.ink-lit}"
  segment-selected:
    backgroundColor: "{colors.on-ink}"
    textColor: "{colors.pacific-ink}"
    rounded: "{rounded.sm}"
    padding: "0 16px"
    height: "44px"
  board:
    backgroundColor: "{colors.ink-raised}"
    textColor: "{colors.on-ink}"
    rounded: "{rounded.md}"
  statement:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.text}"
    rounded: "{rounded.md}"
    padding: "clamp(22px, 3vw, 36px)"
  tag:
    backgroundColor: "{colors.salt-deep}"
    textColor: "{colors.text}"
    typography: "{typography.label}"
    rounded: "{rounded.hair}"
    padding: "5px 9px"
---

# Design System: Pleamar

## Overview

**Creative North Star: "The Conditions Board"**

Pleamar reads like the forecast board surfers check in Tamarindo: a dark, ruled panel of readouts an owner can absorb in a glance. Deep Pacific ink is the board's ground and owns the majority of the page; cool salt-white sections are where the owner sits down to read. One sun-amber is reserved for "now", for sunset and for the primary action, so its appearance always means something is happening or something can be done.

The density is deliberately high and calm: information sits in hairline-ruled rows, tall condensed numerals carry the data, and prose stays in a quiet grotesk. Luxury comes from precision and restraint rather than ornament. Real villa photography is the proof, and every showcase photo carries its care log directly beneath it. The system refuses the category default of full-bleed photo, serif slogan and three airy service cards.

**Key Characteristics:**
- Ink-dominant page: ink sections alternate with salt reading sections, ink owning more than half.
- Condensed uppercase display type (Antonio) for headlines and readouts; Hanken Grotesk for prose.
- Tabular figures everywhere, set on `body`.
- Hairline-ruled rows instead of cards; heavier 1.5px rules open a ruled group.
- State is a drawn mark (done / now / scheduled), never color alone.
- One amber, rationed.

## Colors

A cool, near-monochrome Pacific palette with a single warm accent and a single cool signal.

### Primary
- **Sun Amber**: the only warm color. Primary buttons, the "now" marker and hour on the day rail, the live pulse, sunset readouts, the hero headline's second clause, selection and focus rings. Brightens to **Sun Amber Hover** on button hover.
- **Sun Deep**: amber darkened for legibility on salt grounds (the rating star in the villa facts). Use it whenever amber must appear on light ground.

### Secondary
- **Sea Mark**: the "done" signal on ink grounds (completed events, day-rail pins at rest, check marks in the evaluation section).
- **Sea Mark Deep**: the same signal on salt grounds (care logs under photos, report points), where Sea Mark would fail contrast.

### Neutral
- **Pacific Ink**: the board's ground. Hero, day-of-care, services, evaluation and footer sections; booked nights in the statement calendar.
- **Ink Raised**: panels sitting on ink (the conditions board, the evaluation form, field backgrounds). Panels use it at 92-94% opacity over photography.
- **Ink Lit**: focused field background.
- **On Ink / On Ink Muted**: primary and secondary text on ink. On Ink also fills the selected language toggle and selected segment.
- **Line Ink**: every hairline on ink (rows, table rules, field borders, rail ticks).
- **Salt**: the page ground and reading sections. **Salt Deep**: the process/FAQ band, photo placeholders, tags.
- **Paper**: the owner statement sheet, the only surface lighter than salt.
- **Text / Text Muted / Line**: text, secondary text and hairlines on salt.
- **Error Line / Error Text**: invalid field border and message on the ink form.

### Named Rules
**The One Sun Rule.** Amber means "now" or "act". It never decorates, never fills a section, and never appears as a second hue of emphasis.

**The Ink Majority Rule.** Ink grounds own more than half the page; salt is for reading, not for the default.

## Typography

**Display Font:** Antonio (with Arial Narrow, sans-serif)
**Body Font:** Hanken Grotesk (with system-ui, sans-serif)

**Character:** Tall condensed board lettering against a plain, legible grotesk. The display face reads like a departure board; the body face stays out of its way.

### Hierarchy
- **Display** (600, clamp 3.3-6rem, 0.98, uppercase): the hero H1 only. Its second clause may switch to amber.
- **Headline** (600, clamp 2.6-4.75rem, 1.06, uppercase): section H2s.
- **Title** (600, 1.5rem, 1.05, uppercase): H3s, service group headers (1.375rem), statement title (1.75rem). Process step titles drop to 400.
- **Readout** (Antonio 400, 1.25-3.75rem, line-height 1): numbers and short values: board values, event hours, villa facts, ledger amounts, service frequencies. A small grotesk unit (0.8125rem, 500, muted) may follow.
- **Body** (400, 1.0625rem, 1.6; 1rem under 720px): prose. Paragraphs cap at 56-62ch.
- **Lede** (400, 1.1875rem, 1.55, muted, 56ch): the one paragraph under each section headline.
- **Label** (600, 0.75-0.8125rem, 0.04-0.1em tracking, uppercase): field labels, board header, table column heads, tags.

### Named Rules
**The Readout Rule.** Any number a visitor might compare (times, counts, ratings, money) is set in Antonio at 400 with tabular figures. Prose numbers stay in the body face.

**The Uppercase Belongs to the Board Rule.** Uppercase is for display headings and functional labels only. Body copy and buttons are sentence case.

## Layout

A single centered container (max 1360px) with a fluid gutter (clamp 16-56px). Sections are full-bleed color bands with generous vertical padding (clamp 88-150px); inside them, the head is a two-column split (headline left, lede right, aligned to the bottom) that stacks below 1080px. Content is dense and ruled: rows run 12-16px vertical padding, groups are separated by 28-56px. The villa mosaic uses a 12-column grid (one 8-span lead photo, 4- and 6-span supports, 20px column / 28px row gap) and collapses to one column under 720px. Breakpoints: 1080px (nav links hide, all splits stack, facts go 3-up) and 720px (nav shrinks to 64px, the service table becomes stacked rows, facts go 2-up). The hero fills 100svh with content anchored to the bottom.

## Elevation & Depth

Mostly flat and tonal: depth on ink comes from stepping ink → ink raised → ink lit, and from hairlines. Shadows are rare and soft, used only on objects that physically sit above the page: the amber button, the floating board over the hero photo, and the paper statement over salt.

### Shadow Vocabulary
- **Button lift** (`box-shadow: 0 1px 1px rgba(0,0,0,.12), 0 8px 18px -10px rgba(0,0,0,.45)`): primary button at rest; deepens on hover with a 1px rise.
- **Board float** (`box-shadow: 0 30px 60px -30px rgba(0,0,0,.6)`): the conditions board over photography.
- **Paper sheet** (`box-shadow: 0 1px 2px rgba(11,35,40,.06), 0 24px 60px -28px rgba(11,35,40,.35)`): the statement on salt.
- **Nav rule** (`box-shadow: 0 1px 0 var(--line-ink)`): the solid nav once scrolled; a hairline, not a shadow.

### Named Rules
**The Hairline Over Shadow Rule.** Rows, tables, lists and FAQs separate with 1px rules, never with raised cards. A 1.5px rule in the text color opens a group (facts, steps, ledger total, FAQ, statement head).

## Shapes

Nearly square. Corners are 3px on interactive elements (buttons, fields, segments, language toggle, photos), 4px on panels (board, form, statement, day stage) and 2px on tags and calendar cells. The only circles are the live pulse and the day-rail pins. Form is carried by rules and grids, not by rounded containers.

## Components

### Buttons
Solid, warm, quietly lifted.
- **Shape:** near-square (3px), 52px tall (44px in the nav).
- **Primary:** Sun Amber fill, Pacific Ink text, Hanken 600 1rem, 0 26px padding, trailing arrow icon.
- **Hover / Focus:** brightens to Sun Amber Hover, rises 1px, shadow deepens, arrow slides 3px right; 0.2s on the expo-out ease. Focus is a 2px amber outline offset 3px. Disabled drops to 55% opacity.
- **Ghost:** transparent with a 1px inset currentColor ring; hover adds an 8% white wash.

### Inputs / Fields
- **Style:** Ink Raised fill, 1px Line Ink border, 3px radius, 52px tall, Hanken 500 1rem. Selects carry a drawn chevron in On Ink Muted. Labels sit above in the uppercase Label style.
- **Focus:** border turns amber and the fill steps to Ink Lit; no glow.
- **Error:** border Error Line, message in Error Text below.
- **Segmented choice:** 44px pills of 3px radius with a Line Ink border; selected fills On Ink with ink text.

### Navigation
Fixed, transparent over the hero, turning 96% ink with a hairline once scrolled. Wordmark in Antonio 600 with 0.14em tracking beside an amber wave mark. Links in Hanken 500 0.9375rem at 86% opacity, underline on hover. ES/EN toggle is a bordered two-button group; the pressed language fills On Ink. Below 1080px links hide; below 720px the nav button hides too.

### Tags
Small uppercase Label on Salt Deep, 2px radius. Used to label illustrative content ("Illustrative example" / "Ejemplo ilustrativo").

### Conditions Board (signature)
A raised ink panel with an uppercase header row (title left, live clock with amber pulse right), then readout rows on a 22px / 1fr / auto grid: drawn status mark, muted label, Antonio value right-aligned with optional small unit. A small muted footnote states what is live and what is an example. Rows tick in once on load (0.9s, staggered 80ms, from 8px below with a 4px blur); that is the system's one authored entrance.

### Status Marks
Drawn 1.6px-stroke circle icons: a check for done (Sea Mark), a half-filled disc for now (Sun Amber), a dashed ring for scheduled (On Ink Muted). Always paired with text; color is reinforcement, not the signal.

### Day Rail (signature)
A 48px band ruled into 24 hour ticks with darkened night spans, sea-ringed event pins (amber and scaled 1.35 when active), a dashed amber "now" line with its label, and a 4px On Ink thumb (amber when focused). Scrubbing crossfades a 4:3 photo stage (0.7s opacity, 1.4s settle from 1.04 scale) and opens the matching event row.

### Ruled Tables and Ledgers
Services and the statement ledger are true tables: uppercase column heads over a 1.5px rule, Antonio group headers, frequencies and amounts in readout type, hairline row rules, a faint white wash on row hover. Under 720px rows stack.

### Captioned Photos
Photos (3px radius) carry a bold caption and a care log line beneath, prefixed with a Sea Mark Deep check. On hover the image slowly scales 3.5% over 1.2s.

## Do's and Don'ts

### Do:
- **Do** set every comparable number in Antonio 400 with tabular figures.
- **Do** separate content with 1px hairlines (Line Ink on ink, Line on salt) and open groups with a 1.5px rule in the text color.
- **Do** show state with the drawn done / now / scheduled marks plus text.
- **Do** use Sun Deep and Sea Mark Deep, not Sun Amber and Sea Mark, when those signals sit on salt or paper.
- **Do** label illustrative figures with the Tag component.
- **Do** run transitions on `cubic-bezier(.16,1,.3,1)` and honor reduced motion by removing them entirely.

### Don't:
- **Don't** use amber for anything except "now", sunset and the primary action.
- **Don't** group content in airy rounded cards; use ruled rows and tables.
- **Don't** let color alone carry a status.
- **Don't** add radius beyond 4px or shadows beyond the four listed.
- **Don't** set body copy or buttons in uppercase.
