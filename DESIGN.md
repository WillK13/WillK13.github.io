---
name: "Magellan Research Companion"
description: "A camera-ready research companion where evidence, scholarly typography, and measured restraint carry authority."
colors:
  paper: "#f7f8f6"
  sheet: "#ffffff"
  carbon-ink: "#17201e"
  graphite-muted: "#52615e"
  graphite-quiet: "#5f6c69"
  rule: "#cfd8d5"
  rule-strong: "#879994"
  evidence-teal: "#0d685b"
  evidence-teal-soft: "#dcebe6"
  focus-amber: "#a34f00"
typography:
  display:
    fontFamily: '"Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif'
    fontSize: "clamp(2.8rem, 6.3vw, 5.7rem)"
    fontWeight: 500
    lineHeight: 0.99
    letterSpacing: "-0.035em"
  headline:
    fontFamily: '"Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif'
    fontSize: "clamp(1.85rem, 3.2vw, 2.8rem)"
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: "-0.025em"
  body:
    fontFamily: '"Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif'
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.65
  lead:
    fontFamily: '"Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif'
    fontSize: "clamp(1.25rem, 2vw, 1.55rem)"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: 'ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
    fontSize: "0.75rem"
    fontWeight: 700
    lineHeight: 1.45
    letterSpacing: "0.07em"
rounded:
  focus-only: "2px"
spacing:
  compact: "0.75rem"
  base: "1rem"
  row: "1.5rem"
  section: "clamp(4rem, 7vw, 6.5rem)"
components:
  evidence-link:
    textColor: "{colors.evidence-teal}"
    typography: "{typography.label}"
  model-note:
    backgroundColor: "{colors.evidence-teal-soft}"
    textColor: "{colors.carbon-ink}"
    padding: "0.45rem 0.6rem"
  figure-surface:
    backgroundColor: "{colors.sheet}"
  result-metric:
    textColor: "{colors.evidence-teal}"
    typography: "{typography.label}"
---

# Design System: Magellan Research Companion

## Overview

**Creative North Star: "The Camera-Ready Companion"**

Magellan translates the composure of proceedings front matter into a responsive research microsite. The system feels exact, quiet, and visibly academic: crisp paper, carbon ink, graphite rules, generous margins, and one restrained evidence color let the research figures and qualified measurements carry the page.

The interface avoids promotional hero language, conversion patterns, ornamental cards, and decorative illustration. Its only signature mark is a small globe crossed by an orbital arrow, connecting geographic movement to the research subject without competing with the evidence.

**Key Characteristics:**

- Paper-like surfaces with square, rule-led structure.
- Editorial serif reading type paired with plain sans-serif metadata.
- Deep teal reserved for evidence, links, and the migration mark.
- Wide scholarly layouts that collapse into one disciplined reading column.
- Figures presented at full readable width with experiment context attached.

## Colors

The palette is nearly achromatic, with cool graphite neutrals and a single restrained teal voice for evidence.

### Primary

- **Evidence Teal** (`evidence-teal`, #0d685b): identifies research links, measured result numerals, action labels, venue metadata, and the orbital globe mark.
- **Soft Evidence Wash** (`evidence-teal-soft`, #dcebe6): supports selected text and compact technical notation without becoming a card background.

### Neutral

- **Paper** (`paper`, #f7f8f6): the cool page ground surrounding all research content.
- **Sheet White** (`sheet`, #ffffff): the clean backing used behind supplied figures.
- **Carbon Ink** (`carbon-ink`, #17201e): titles and primary reading text.
- **Muted Graphite** (`graphite-muted`, #52615e): explanations, captions, and supporting copy.
- **Quiet Graphite** (`graphite-quiet`, #5f6c69): qualifications and deliberately recessive notes.
- **Graphite Rule** (`rule`, #cfd8d5): internal divisions and evidence-row structure.
- **Strong Graphite Rule** (`rule-strong`, #879994): major section, masthead, and footer boundaries.
- **Focus Amber** (`focus-amber`, #a34f00): keyboard focus only, chosen to remain distinct from the teal evidence voice.

**The One Evidence Color Rule.** Deep teal is the only expressive page color; it signals evidence and navigation rather than decoration.

**The Qualification Contrast Rule.** Supporting copy may recede to graphite, but quantitative qualifications must remain clearly readable against paper.

## Typography

**Display Font:** Iowan Old Style, falling back through Palatino and Georgia.

**Body Font:** Iowan Old Style, falling back through Palatino and Georgia.

**Label Font:** The platform UI sans-serif stack, falling back to Segoe UI and sans-serif.

**Character:** The serif carries the pace and authority of a paper; the sans-serif makes metadata, navigation, measurements, and running labels immediately scannable. Neither family is used as ornament.

### Hierarchy

- **Display** (500, responsive 2.8–5.7rem, 0.99 line height): the paper title only, balanced at a compact measure of roughly 15 characters.
- **Headline** (500, responsive 1.85–2.8rem, 1.1 line height): section titles with modest negative tracking.
- **Lead** (400, responsive 1.25–1.55rem, 1.5 line height): the concise opening contribution statement.
- **Body** (400, 1rem, 1.65 line height): sustained reading copy, generally held to 70 characters or fewer.
- **Label** (700, 0.75rem, 0.07em tracking): uppercase figure labels and action names; metadata links use the same sans-serif family at context-appropriate sizes.

**The Two-Voice Rule.** Serif communicates the research argument; sans-serif organizes the apparatus around it.

**The Numeric Authority Rule.** Key measurements use tabular numerals, strong weight, and evidence teal so comparison is immediate without inflating the surrounding prose.

## Layout

The page uses a centered container capped at 1180px, with 1.5rem side gutters on wide screens and 1rem gutters below 760px. Major sections are separated by strong graphite rules and use fluid vertical padding (`section`) rather than boxed containers.

Desktop composition relies on asymmetric two-column grids: headings or labels occupy the narrower left track while the reading argument sits in the wider right track. Result rows, section introductions, captions, and the citation reuse that alignment so the reader learns one spatial grammar. The paper header gives the title the dominant track and keeps authorship and venue metadata compact at the edge.

At 760px and below, all multi-column reading structures become a single column, the three decision actions stack with horizontal dividers, the technical model becomes linear, and two middle navigation links are hidden while the first and last anchors remain. Type stays generous and figures remain full width. Reduced-motion preference disables smooth scrolling.

**The Open Page Rule.** Create hierarchy with measure, alignment, whitespace, and rules—not with nested cards.

## Elevation & Depth

The system is flat by design and uses no shadows. Depth comes from the slight contrast between cool paper and white figure surfaces, from strong and quiet rule weights, and from whitespace around evidence. Interactive states change underline color or text color; they do not lift elements off the page.

**The Flat Evidence Rule.** Research artifacts remain on the reading plane; never imply importance through drop shadows or floating panels.

## Shapes

The form language is square and camera-ready. Sections, figures, result rows, and technical notes have no corner rounding. The sole radius token is a subtle 2px accommodation on keyboard focus outlines, not a component silhouette. The globe mark uses circles because geography is intrinsic to its meaning; that curvature should not spread into pill controls or rounded containers.

**The Square Page Rule.** Borders terminate cleanly and surfaces remain square; curved geometry belongs to the orbital mark alone.

## Components

### Wordmark

- **Character:** A compact sans-serif name paired with a 2rem line-drawn globe and orbit arrow.
- **Color:** Evidence teal for the mark and carbon ink for the name.
- **Behavior:** Links to the top without underline decoration; the mark remains the only illustrative signature.

### Navigation

- **Character:** Quiet running links in muted graphite, set in compact sans-serif type.
- **Default / Hover:** No underline at rest; hover moves the text to carbon ink.
- **Focus:** A 2px focus-amber outline with 4px offset.
- **Mobile:** Preserve the first and last anchors and remove the two middle links below 760px.

### Evidence Links

- **Character:** Compact, semibold sans-serif links in evidence teal.
- **Behavior:** A fine, offset underline becomes fully opaque on hover; external and download actions retain their plain-text glyph cues.
- **Focus:** Use the shared high-contrast amber focus outline.

### Result Rows

- **Structure:** Three equal columns form a single scholarly results table, separated by graphite rules rather than card frames.
- **Metric:** Oversized tabular numerals in evidence teal lead each column, with the result label and experiment-specific qualification attached directly below.
- **Mobile:** Stack the results as three ruled records while preserving the oversized numeric emphasis.

### Decision Flow

- **Structure:** Three equal, open sections for Continue, Pause, and Migrate. Each begins with its own evidence-teal top rule and ends with a quiet graphite rule; generous gaps keep them distinct without card frames.
- **Labels:** Compact sans-serif headings over muted serif explanation.
- **Mobile:** Stack the actions with the same independent ruled-section treatment.

### Model Note

- **Structure:** A two-column explanatory section: a plain-language introduction on the left and the score, objective legend, and constraints on the right.
- **Technical Highlight:** Only the displayed equation receives the soft evidence wash; the surrounding component stays on open paper between strong graphite rules.
- **Mobile:** Collapse the explanation and equation to one column, then stack the three objective definitions.

### Figure Records

- **Structure:** Each full-width figure or recorded replay sits on sheet white, followed by a three-part caption for label, interpretation, and source-file link.
- **Replay:** Use native video controls, a representative extracted poster frame, explicit language distinguishing recorded simulation from live execution, and white fallback text on the dark video ground.
- **Boundary:** A quiet graphite rule begins each record; no card frame or shadow encloses it.
- **Mobile:** Caption parts stack in reading order.

## Do's and Don'ts

### Do:

- **Do** use strong rules and generous section spacing to make the page scan like a proceedings companion.
- **Do** keep experiment context attached to every quantitative result and figure.
- **Do** reserve evidence teal for links, measurements, action labels, venue metadata, and the orbital mark.
- **Do** preserve the serif/sans division between research argument and interface metadata.
- **Do** let supplied figures occupy the full readable width of the content container.

### Don't:

- **Don't** introduce promotional heroes, conversion calls to action, feature-card grids, or commercial landing-page language.
- **Don't** add shadows, pill shapes, rounded cards, gradients, or competing accent colors.
- **Don't** use the globe-and-orbit motif as repeating decoration; it is a singular identifying mark.
- **Don't** separate a reported measurement from its baseline or experimental qualification.
- **Don't** compress long-form reading beyond a comfortable 70-character measure or shrink figure evidence into thumbnails.
