---
name: Richmond Equipment Rental
description: An active job site you can dig in. Fence green over a bank of real soil, equipment yellow on the controls, a grade laser's red line across the dirt.
colors:
  site: "#17352d"
  yellow: "#f2b705"
  yellow-hi: "#ffc928"
  laser: "#ff5a45"
  soil: "#3d2a1b"
  soil-2: "#4a3322"
  soil-deep: "#33231a"
  cream: "#f4ecda"
  cream-dim: "#d8cbb0"
  ink: "#1d1a12"
  placeholder: "#b7a98c"
  error-text: "#ffb4a8"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2.75rem, 13.2vw, 6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2rem, 8.5vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1.6rem"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  numeral:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "2.4rem"
    fontWeight: 900
    lineHeight: 0.9
  row:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 800
    lineHeight: 1.32
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(1rem, 4.4vw, 1.25rem)"
    fontWeight: 400
    lineHeight: 1.45
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1rem"
    fontWeight: 700
    lineHeight: 1.4
  button:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(0.95rem, 4.3vw, 1.05rem)"
    fontWeight: 800
    lineHeight: 1.1
rounded:
  control: "10px"
  button: "12px"
  photo: "16px"
  panel: "18px"
  round: "50%"
spacing:
  gutter: "20px"
  gutter-wide: "36px"
  stack: "12px"
  field: "18px"
  section: "44px"
  section-wide: "64px"
components:
  button-fill:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.button}"
    padding: "0 16px"
    height: "58px"
  button-fill-hover:
    backgroundColor: "{colors.yellow-hi}"
    textColor: "{colors.ink}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.cream}"
    typography: "{typography.button}"
    rounded: "{rounded.button}"
    padding: "0 16px"
    height: "58px"
  service-row:
    textColor: "{colors.cream}"
    typography: "{typography.row}"
    padding: "12px 0"
    height: "64px"
  service-arrow-hover:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.round}"
    size: "40px"
  estimate-panel:
    rounded: "{rounded.panel}"
    padding: "22px 18px 24px"
  input:
    textColor: "{colors.cream}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "13px 14px"
    height: "52px"
  chip:
    textColor: "{colors.cream}"
    rounded: "{rounded.control}"
    padding: "8px 14px"
    height: "44px"
  chip-selected:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
---

# Design System: Richmond Equipment Rental

All values live in one file, `index.html`. Line numbers below are as shipped (2026-10-17) and will drift as the file is edited; the selector or constant name is the stable handle.

## Overview

**Creative North Star: "The Open Trench"**

The page is an active job site seen from the side, and scrolling goes underground. The top is construction-fence green with the soil bank in the hero; below that, services, the estimate steps and the form sit on successively deeper soil layers separated by hand-wavy strata seams; the work photo stands on a second dirt bank; the footer is the deepest soil. Nothing is ever black: the bottom of the page is still dirt.

The interaction is the identity. The soil is drawn on canvas, slumps to its angle of repose, throws grains, and an excavator bucket follows the finger or mouse, digs, carries and dumps. Left alone, the hero bucket grades the bank to a rotary laser's red line by itself. Everything else on the page is deliberately plain and phone-first so the dirt carries the character and the number stays easy to hit.

Type is the system sans at heavy weight, uppercase and tight, like stencil on a machine; controls are equipment yellow; laser red is reserved for the "you are touching this" signal on form controls and for the laser beam itself.

**Key Characteristics:**
- Fence green surface, soil-brown strata below, no black grounds anywhere.
- Equipment yellow for every primary control and every emphasized numeral or word.
- Laser red only for form hover/focus outlines and the canvas laser beam.
- System font stack, 900 uppercase display, generous 16px body.
- Two interactive canvas dirt scenes; the rest is flat, quiet and touch-sized (44px minimum targets).

## Colors

Colors from the trade, not from a brand (none exists): fence green, equipment yellow, soil browns, grade-laser red, sun-faded cream text. Tokens live on `:root` at `index.html` lines 20-34.

### Primary
- **Equipment Yellow** (`--yellow`): every filled button, the selected chip, hovered service arrows, step numerals, the yellow word in the hero headline, Who headings, the phone icon, link hover color, text selection, the caret, and the default focus ring. Matches the Wacker Neuson carrier in the work photo.
- **Yellow, Lit** (`--yellow-hi`): hover state of the filled button only.

### Secondary
- **Grade-Laser Red** (`--laser`): border on hovered/focused inputs, textarea, chips and the copy button; outline on the hovered/focused submit button; the canvas laser beam and emitter. It never fills a surface and never colors text.

### Neutral (grounds, darkest at the bottom)
- **Fence Green** (`--site`): page background, hero and the proof section. The hero adds a one-off lighter top (`#1b3d34` to `--site`, line 68). `--site-2` is defined on `:root` but unused, so it is not part of the system.
- **Soil** (`--soil`): services section and the close section. It equals the bottom stop of the canvas dirt gradient, so the hero bank flows straight into the first section with no seam.
- **Soil, Second Layer** (`--soil-2`): the How-estimates section.
- **Deep Soil** (`--soil-deep`): footer.
- **Cream** (`--cream`): primary text, outline-button text, input text.
- **Cream, Dim** (`--cream-dim`): secondary copy (promise line, step detail, notes, footer).
- **Ink** (`--ink`): text on yellow; at 28% alpha it is the estimate panel's recessed ground.
- **Placeholder** and **Error Text**: input placeholder and the inline validation message. Functional only.

Cream at low alpha is the system's line and fill material: 14% for service-row rules, 22% for control borders at rest, 30% for the copy button border, 6-10% for input and arrow fills.

### Named Rules
**The No Black Ground Rule.** No section, panel or footer is black or near-black. The deepest ground is Deep Soil; when a darker layer is needed, go browner, not blacker.

**The Laser Means Touch Rule.** Laser red appears only where the visitor's pointer or focus is on a form control, plus the laser in the canvas. Don't use it for errors (errors use Error Text), decoration or headings.

**The Yellow Is a Control Rule.** Yellow fills are things you press. Yellow text is reserved for emphasis that echoes the controls (the headline word, numerals, Who headings), never body copy.

## Typography

**Display Font:** system stack `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif` (`--font`, line 33)
**Body Font:** the same stack

**Character:** One family, two voices: 900-weight uppercase at 0.95 line-height for anything that is a heading, 400-weight sentence case at 1.55 for the owner talking. The heavy uppercase reads as machine stencil without loading a font.

### Hierarchy
- **Display** (hero headline, `.hero h1`, line 72): max 11ch on phone, 12ch at 1024px+. One word wrapped in `<em>` turns yellow, no italics.
- **Headline** (every `h2`, line 43): section titles, 28px below.
- **Title** (`.who h3` at 1.6rem yellow; `.estimate h3` at 2rem): sub-headings. All h1-h3 share weight, case, tracking and leading from line 42.
- **Numeral** (`.steps li::before`, line 106): the yellow step counter.
- **Row** (service links at 800, step leads at `b` 1.25rem): list items you read first.
- **Lead** (`.promise`, line 74): the single promise line under the hero headline, max 34ch (40ch at 1024px+).
- **Body** (`body`, line 37): 16px, max 40ch in Who and Close copy.
- **Label** (`.field>span`, `.legend`, line 120): form labels at 700; hints in `small` at 400 dim.
- **Button** (`.btn`, line 48): 800 weight, sentence case.

### Named Rules
**The System Stack Rule.** The system font stack is a house decision, not a placeholder: no webfont requests, instant first paint inside Facebook's in-app browser. Character comes from weight (900), case and tight tracking. Don't add a display face.

**The 1rem Floor Rule.** Nothing on the page is smaller than 0.875rem (the "Poconos, PA" line under the name); all helper, error and footer text is 1rem.

## Layout

- **Container:** `.wrap` max 1180px, side padding `--gutter` (20px phone, 36px from 700px; set at line 172).
- **Breakpoints:** 700px (buttons side by side, Who in two columns, larger header type, roomier form panel) and 1024px (hero becomes ~92svh with the dirt canvas full-bleed behind the copy, services and Who side by side, How steps and the form side by side with the steps column sticky, photo crops to 16:9). Both blocks are at lines 171-199.
- **Stacking order (story):** header (name + number) → hero headline, promise, two buttons → dirt bank → What I do (rows) + Homeowners/Contractors → How estimates work (steps, area) + estimate form → Recent work (photo standing in a dirt bank) → Facebook button, close headline, Text me, call line → footer.
- **Rhythm:** sections pad roughly 38-52px top and 56-64px bottom on phone, 52-84px top and 80-90px bottom on desktop. Within blocks, the working steps are 12px (button stack), 18px (between fields), 22-26px (between steps / Who items), 44px (steps to area). Spacing is set per selector, not from a scale; keep new values near these.
- **Desktop hero:** the canvas sits `position:absolute; inset:0` behind the copy; the scene measures the headline, promise and buttons on resize and keeps both the dirt and the autoplay bucket at least 40px clear of them (`clearX`/`clearH`, lines 453-464). Copy has `pointer-events:none` except its links so the bank is draggable around it.

**The Phone-First Rule.** Every layout decision is made for a ~390px phone first; desktop only spreads the same stack into columns. Buttons stack full width on phone.

## Elevation & Depth

Depth is geological, not stacked cards. Layers are conveyed by ground color going darker and browner as you scroll, joined by organic seams, plus the canvas soil's own gradient and topsoil band. Shadows are rare and soft.

### Shadow Vocabulary
- **Button lift** (`0 6px 18px -6px rgba(0,0,0,.45)`): filled yellow buttons only.
- **Photo drop** (`0 18px 40px -18px rgba(0,0,0,.6)`): the work photo only.
- **Bucket contact shadow** (canvas, line 752): an ellipse on the soil under the bucket that softens and widens as it lifts.

### Named Rules
**The Strata Rule.** Adjacent sections meet at a seam, not a straight edge: the seam is the upper section's color drawn as a wavy 28px edge over the top of the lower one. New sections take the next soil tone and a seam.

**The Soft-Only Shadow Rule.** Shadows are blurred and negative-spread. No hard offset shadows.

## Shapes

Softly rounded controls on an organic ground. Controls (inputs, chips, copy button) are 10px; buttons and the composed-message box 12px; the work photo 16px on its top corners only, since its bottom is buried in dirt; the estimate panel 18px; service arrows are circles. Borders are 2px on every interactive control, 1px for row dividers. Everything organic (seams, soil profile, the static fallback bank's clip-path polygon at line 81) is irregular on purpose.

## Components

### Buttons
Big, blunt, thumb-sized.
- **Shape:** 12px radius, 58px min height, 2px yellow border always, inline 22px stroke SVG icon with 10px gap (`.btn`, lines 47-55).
- **Fill:** yellow ground, ink text, button lift shadow. Used for "Text me photos for an estimate", the form submit and "Text me".
- **Line:** transparent ground, cream text, yellow border. Used for "Fill out the estimate form" and the Facebook button.
- **Hover / Focus:** fill goes to Yellow, Lit; line gets a 12% yellow wash; 1px press-down on `:active`; default focus ring is 3px yellow, offset 3px (line 44). Inside the estimate form only, hover and focus add a 3px laser outline offset 2px (line 138).
- **Layout:** full width stacked on phone; auto width side by side with 28px padding from 700px.

### Service Rows with Arrow
The services list is a set of tap targets, each one opening a pre-written text about that job.
- 64px min rows, 1.25rem 800-weight label, 1px cream-14% rules top and bottom (lines 87-95).
- A 40px circular arrow at the right, cream-10% fill at rest; on hover/focus the circle turns yellow with ink arrow. Focus puts the 3px yellow ring on the arrow instead of the row.
- The row itself never highlights; only the arrow responds.

### Estimate Form
- **Panel:** ink at 28% on the soil layer, 18px radius, 22px/18px padding (32px from 700px) (line 116).
- **Inputs / Textarea:** 52px min (textarea 110px, vertical resize), 2px cream-22% border, cream-6% fill, 10px radius, 16px text so iOS doesn't zoom (lines 122-126).
- **Hover and Focus:** border turns laser red and the fill lifts to 9%; the browser outline is replaced by that border.
- **Chips** (job type, multi-select checkboxes): 44px min, 10px radius, 2px cream-22% border, 600 weight. Hover or keyboard focus turns the border laser red; checked fills yellow with ink text and keeps the laser border on hover (lines 129-136).
- **Errors:** Error Text, 600 weight, shown under the field, announced politely. Only location and description are required.
- **Composed message:** after submit, a cream-7% box with the written message (selectable) and a Copy button with a 2px cream-30% border that turns laser on hover/focus. This is the desktop fallback when `sms:` can't open.

### Step Numerals
How-estimates steps are an ordered list with a CSS counter: a 44px left column holding a 2.4rem 900 yellow numeral, then a 1.25rem bold lead and a dim detail line (lines 104-108).

### Header and Contact Line
Name stacked over "Poconos, PA" on the left, the phone number with a yellow handset icon top right (lines 58-64). Number scales to 1.25rem from 700px. There is no other navigation.

### Strata Seams (signature)
Inline SVGs (`#seam1` at the top of How, `#seam2` at the top of Proof), 28px tall, stretched with `preserveAspectRatio="none"`. Drawn once by script at lines 389-400 from three summed sines.
- **Knobs:** the seed per seam (`1.3`, `4.1`, line 398-399) changes the wave; amplitudes `5`, `3`, `1.5` and frequencies `.011`, `.037`, `.09` (line 394) set roughness; baseline `14` sets depth.
- Fill is read from the CSS custom property of the section above (`--soil`, `--soil-2`), so recoloring a section recolors its seam.

### Dirt Scenes (signature)
Two canvas scenes share one animation loop (lines 402-830).
- **Hero bank** (`#dirtHero`): autoplay on, laser on, keeps clear of the headline on desktop. 210-250px tall on phone (`.dirt-hero`, line 76), full hero behind the copy from 1024px.
- **Photo bank** (`#dirtClose`): autoplay off, laser off, its grade sits 14px above the photo's bottom so the photo looks planted; the bucket only appears while you dig. 150px tall, overlapping the photo by 62px (190px / 80px on desktop, lines 152 and 197). Vertical page scroll is preserved on touch (`touch-action: pan-y`).
- **Static fallback:** a clip-path soil silhouette (`.still`, line 80) shows until the canvas is ready and remains for reduced motion, where each scene draws one still frame.
- **Physics knobs, `TUNE` (lines 404-415):**
  - `GRADE` (0.40): laser line height as a share of canvas height (capped at 150px on desktop, line 452).
  - `REPOSE` (0.75): steepest slope soil will hold; higher = steeper piles.
  - `RELAX` (5): slump passes per frame; higher = soil settles faster.
  - `SPRING` (140) / `DAMP` (13): how hard and how smoothly the bucket chases the finger.
  - `IDLE_MS` (2600): untouched time before the hero bucket resumes grading.
  - `GRAIN_VOL` (5): soil volume per flying grain; lower = more grains.
  - `DIG_TILT` (-0.55), `CARRY_TILT` (0.22), `DUMP_TILT` (-2.1): bucket angles in radians for digging, carrying and dumping.
- **Other knobs in `resize()` (lines 441-476):** column width 3px phone / 4px desktop (`cw`), bucket radius 17-30px (`r`), bucket capacity (`cap`), device-pixel cap 1.5, grain limit 500 phone / 1100 desktop. The terrain bumps, spoil pile and trench are generated in `profile()` (lines 478-502).
- **Soil material:** body gradient `#80583a → #6a4629 → #4f3522 → #3d2a1b` (line 535), shared 256px grain-and-pebble tile (lines 506-528), darker topsoil stroke along the surface (lines 696-698), flying-grain colors `GRAIN_COLORS` (line 683). The gradient's last stop must stay equal to `--soil`.
- **Bucket** (`drawBucket`, lines 745-805): steel side plate gradient `#5d6062 → #2f3133`, rib, wear strip and tooth, yellow pins, a yellow stick that fades out in its last 28px, a dark cylinder with a chrome rod. Faces its direction of travel. Heaped load shows in the mouth. A user dumps by holding the bucket still in the air for 0.35s.
- **Rotary laser** (`drawLaser`, lines 712-742): a yellow head with a blinking red emitter on a grey tripod near the right edge (24px in on phone, 40px on desktop), modeled on the laser level in the work photo. The beam is a 1.2px laser-red line at 55% alpha at grade height that stops at the first soil face or at the bucket, with a small glowing hit spot.
- **Autoplay** (`autoplay`, lines 549-584): cut the highest spot above grade, carry and dump it into the lowest; once level, dig a trench and heap the spoil beside it so the next round has work. The bucket never leaves the canvas.

## Do's and Don'ts

### Do:
- **Do** keep the phone number visible top right on the first screen, as the only number shown there; the hero's two buttons are text and form, phone first.
- **Do** put new sections on the next soil tone with a strata seam, per The Strata Rule.
- **Do** use the 2px laser-red border for hover and focus on any new form control, and the 3px yellow ring for focus everywhere else.
- **Do** keep every tap target at 44px or taller and every text size at 1rem or larger (except the 0.875rem brand subline).
- **Do** keep the email address in the footer only, and the Facebook link as the button directly under the work photo's dirt bank (plus the footer).
- **Do** tune the dirt from `TUNE` first; change `profile()` or `resize()` only for terrain shape or density.
- **Do** keep the canvas soil gradient's last stop equal to `--soil` so the bank flows into the first section.

### Don't:
- **Don't** add a webfont; the system font stack is on purpose.
- **Don't** add a sticky or fixed call bar. (The desktop steps column is sticky inside its grid; that is not a bar.)
- **Don't** use black or near-black grounds anywhere, per The No Black Ground Rule.
- **Don't** repeat the phone number elsewhere in the first screen, or show the email outside the footer.
- **Don't** use laser red as a fill, for text, or for errors.
- **Don't** put kicker or eyebrow labels above headings; the h2 stands alone.
- **Don't** use hard offset shadows.
