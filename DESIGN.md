---
name: Richmond Equipment Rental LLC
description: Calm paper and fence-green bands, one equipment-yellow fill, for a one-man dirt-work outfit in the Poconos.
colors:
  paper: "#f5f6f2"
  card: "#ffffff"
  field: "#e5eae3"
  ink: "#10271f"
  body: "#28382f"
  soft: "#4c5a51"
  fence-green: "#1f4a3c"
  deep-green: "#10271f"
  on-dark: "#f5f7f3"
  on-dark-soft: "#c6dccc"
  equipment-yellow: "#f2b705"
  equipment-yellow-hover: "#ffc929"
  yellow-ink: "#805c00"
  focus: "#1f4a3c"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  phone-display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 9vw, 52px)"
    fontWeight: 400
    lineHeight: 1
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "24px"
    fontWeight: 400
    lineHeight: 1.08
  row:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(20px, 5.4vw, 24px)"
    fontWeight: 400
    lineHeight: 1.15
  step:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "21px"
    fontWeight: 400
    lineHeight: 1.2
  button:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.15
  field-label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  promise:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.7vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.02em"
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter-desktop: "40px"
  card-pad: "24px"
  block: "32px"
  band-phone: "64px"
  band-desktop: "96px"
  container: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.equipment-yellow}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.equipment-yellow-hover}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-copy:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "44px"
  eyebrow:
    backgroundColor: "rgba(16,39,31,.06)"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
  eyebrow-on-dark:
    backgroundColor: "rgba(255,255,255,.12)"
    textColor: "{colors.on-dark}"
  card-who:
    backgroundColor: "{colors.card}"
    textColor: "{colors.body}"
    rounded: "{rounded.card}"
    padding: "{spacing.card-pad}"
  input-text:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "#ffffff"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
    width: "600px"
  service-row:
    textColor: "{colors.on-dark}"
    typography: "{typography.row}"
    padding: "12px 0"
    height: "72px"
  row-arrow:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    size: "44px"
  row-arrow-hover:
    backgroundColor: "{colors.equipment-yellow}"
    textColor: "{colors.ink}"
  step-number:
    backgroundColor: "{colors.equipment-yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-text:
    backgroundColor: "{colors.equipment-yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: Richmond Equipment Rental LLC

## Overview

**Creative North Star: "The Graded Lot"**

The page reads like the job photo it is built from: a cleared, level site, a green construction fence, one yellow machine. Full-bleed bands alternate light and dark so each section is unmistakable, and everything inside them is soft-cornered, borderless and calm. The system is Ellie's house "calm band style" (learned from lpmr.co.uk), coloured from the client's own photo because the business has no logo or brand colours: the fence gives the green, the Wacker Neuson loader gives the yellow.

Density is low and phone-first. One column on phones, a 1160px container on computers, generous 64px/96px band padding, short rows instead of dense grids. Depth comes from band colour, a white card on a paper ground, and the hero photo, not from shadows. Motion is limited to two owner-chosen moves: the hero headline's letter bounce-in and one 12px fade-up for content below the first screen.

Several choices here are owner-chosen exceptions to Impeccable's defaults and are part of the system, not drift: the eyebrow pills, Cal Sans as the display webfont, the hero H1 letter bounce-in, and the faint diagonal-line texture on deep-green bands. Each is bounded by rules below.

**Key Characteristics:**
- Paper, fence-green and deep-green full-bleed bands, alternating light and dark.
- Equipment yellow is the only warm colour and is used as a fill; it becomes the darker yellow-ink only when it must be text on a light ground.
- Cal Sans (weight 400) for every heading, button, row and field label; the system stack at 16/1.7 for running text.
- Soft, borderless shapes: 24px cards, full pills for buttons, chips and eyebrows, 10px fields on their own tinted fill.
- Flat surfaces; the floating text circle is the only element with a shadow.
- The client's real job photo carries the hero: a bottom strip on phones, full-bleed under a left-dark gradient from 760px.

## Colors

A cool, slightly green-grey paper and two photo-sourced greens, with a single saturated equipment yellow doing all the warm work.

### Primary
- **Equipment Yellow** (equipment-yellow): the loader's paint. A fill only: the primary button, the step numbers, the floating text circle, the service-row arrow on hover, the eyebrow's dot, text selection. Text on it is always Ink (8.7:1). On dark bands and the hero it may also colour a heading's last phrase, the Facebook glyph and the phone glyph in the close band.
- **Bright Yellow** (equipment-yellow-hover): the primary button's hover fill on pointer devices only.
- **Yellow Ink** (yellow-ink): yellow when it has to be text or a glyph on a light ground: the header phone icon and its hover colour, and the `.accent` phrase if one ever sits on paper (5.6:1 on paper).

### Secondary
- **Fence Green** (fence-green): the construction fence in his photo. The services band, the closing call band, and the Facebook row's fill on paper. The same value is the Focus token: the outline and hover border on light surfaces and the text caret in fields.

### Tertiary
- **Deep Green** (deep-green): the hero ground and overlay base, the "How estimates work" band and the footer. Always carries the diagonal texture. Shares its value with Ink.

### Neutral
- **Paper** (paper): page ground, header, and the light bands. Also the theme-color.
- **Card White** (card): the who-cards and the form card; the only pure white surface.
- **Field Mist** (field): inputs, unselected chips, the sent-fallback panel and the photo placeholder. Fields sit on this fill, never on a border.
- **Ink** (ink): headings on light, text on yellow, selected chips, the copy button's outline.
- **Body** (body): running text on light (11.4:1 on paper).
- **Soft** (soft): ledes, small hints, placeholders, the wordmark sub-line, the after-submit note (6.7:1 on paper).
- **On Dark** (on-dark): headings, row text and links on green bands. The hero H1 is pure white.
- **On Dark Soft** (on-dark-soft): running text on green bands (6.9:1 on fence green, 10.9:1 on deep green).
- **Row Rule** (`rgba(255,255,255,.14)`): the 1px hairlines between service rows on fence green; the only divider in the system.
- **Error** (error): field error text and the bad-field border.

### Named Rules
**The Fill-Not-Text Rule.** Equipment yellow is a surface, not a text colour on light grounds. On paper or white it becomes Yellow Ink; on yellow, text is Ink. White on yellow is never used.

**The Accent-Phrase Rule.** A heading's closing phrase may turn yellow only on a dark band or the hero ("in the Poconos.", "take on.", "work."). Light-band headings stay solid Ink.

**The Texture-Whisper Rule.** Deep-green surfaces carry `repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`. Owner-chosen exception: it stays at about 4% white or fainter so it never reads as lines through text, and it never goes on paper or fence green.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** System stack (with -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans is a rounded, slightly condensed geometric that looks sturdy at one weight; set at 400 throughout, it gives every heading, button and row label the same friendly-workman voice. The system body keeps running text native and fast on the Facebook in-app browser where most visitors arrive.

Cal Sans loads from Google Fonts (`display=swap`, with preconnect). It is an owner-chosen exception (calm band style, 2026-10-19) to the system-stack-only default; the page loads one family at one weight and nothing else.

### Hierarchy
- **Display** (400, `clamp(42px, 12vw, 80px)`, 1.02): the hero H1 only, white, max 12ch. In landscape phones (760px+ wide, 520px or less tall) it drops to `clamp(40px, 11vh, 64px)` with no width cap.
- **Headline** (400, `clamp(30px, 7.6vw, 48px)`, 1.08, -0.005em, balanced): every section H2.
- **Phone Display** (400, `clamp(30px, 9vw, 52px)`, 1): the big tap-to-call number in the closing band.
- **Title** (400, 24px): who-card H3s.
- **Row** (400, `clamp(20px, 5.4vw, 24px)`, 1.15): service rows; the Facebook row uses `clamp(19px, 5.2vw, 22px)`/1.2.
- **Step** (400, 21px, 1.2; 22px from 1024px): step headings in "How estimates work"; footer name and wordmark also sit at 21px.
- **Button** (400, 18px, 1.15): all pill buttons. Field labels and legends use Cal Sans 17px/1.2; the header phone 17px (20px from 760px); the wordmark 21px (24px from 760px).
- **Promise / Lede** (system, `clamp(17px, 4.7vw, 20px)`/1.5 at 32ch, 36ch from 760px; `clamp(17px, 4.6vw, 19px)`/1.7 at 38ch): the hero promise line and section ledes.
- **Body** (system 400, 16px, 1.7): running text, inputs (16px so iOS doesn't zoom), chips, the service note. 18px for the service-area line, 15px for errors, the after-submit note and the composed message.
- **Label** (system 500, 14px, 0.02em, sentence case): eyebrow pills. The wordmark sub-line is the one uppercase setting (system 600, 11px, 0.08em) and belongs to the wordmark lockup only.

### Named Rules
**The One-Weight Display Rule.** Cal Sans is only ever set at 400. Emphasis comes from size and colour, never from bolding the display face.

**The Display-For-Doing Rule.** Anything a visitor taps or answers (buttons, rows, phone numbers, field labels, step headings) is in Cal Sans; anything they read at length is in the system body.

## Layout

A single 1160px container (`.wrap`) with a 20px gutter on phones and 40px from 760px. Sections are full-bleed bands with 64px vertical padding on phones and 96px from 760px; band order is hero (deep green) → paper → fence green → paper → deep green → paper → fence green → footer (deep green). Inside a band, a heading group sits at most 640px wide with 16px between eyebrow, heading and lede, and the first content block follows 32 to 36px below.

Breakpoints, as used: 380px and below (chips tighten to 14px side padding); 760px (desktop gutter, band padding, photo goes full-bleed, hero buttons go side by side at 240px min width, who-cards two-up with 24px gap); 760 to 1023px (tablet hero overlay stays dark further right); 760px+ and 520px tall or less (landscape phone hero compresses so the buttons stay on the first screen); 1024px (service rows two columns with a 40px gap, work band becomes photo-left 1.4fr / heading and Facebook row right 1fr, form band becomes sticky heading left 1fr / form right 1.2fr with 64px gap, steps go three-up with 40px gap, closing band puts the big number on the right).

On phones the hero photo is a strip along the hero's bottom edge, `--strip: clamp(190px, 50vw, 300px)` tall, and the copy sits on plain deep green above it, padded 56px top and strip + 8px bottom. From 760px the photo fills the band and the copy is padded 104px top, 120px bottom.

Safe areas are respected: the header top padding, footer bottom padding (96px + inset, leaving room for the float) and the float's position all add `env(safe-area-inset-*)`.

## Elevation & Depth

The system is flat. Depth is conveyed by band colour changes, a white card lifted against paper by tone alone, and the hero's photo-under-gradient. There are no borders on cards or fields and no shadows on any in-flow element.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(8,24,18,.3)`): the floating text circle only, the one element that sits above the page. Its focus state adds a 3px Ink ring inside the yellow outline.

### Hero overlays
- **Phone**: `linear-gradient(180deg, deep-green until the strip starts, rgba(16,39,31,.55) at 55% into the strip, rgba(16,39,31,.25) at the bottom)`.
- **Desktop (1024px+)**: `linear-gradient(90deg, rgba(16,39,31,.93) 0%, .86 at 45%, .42 at 100%)`, darkest behind the words on the left.
- **Tablet (760 to 1023px)**: `.93 0%, .88 at 70%, .6 at 100%`, because the words run past the middle.

### Named Rules
**The Tone-Not-Shadow Rule.** Surfaces separate by colour (paper, white, field mist, fence green, deep green). A shadow appears only on something that floats over the page.

## Shapes

Three radii, all soft: 10px for text fields, 24px for cards, the form and the work photo, and full pills (999px) for buttons, chips, eyebrows, the copy button, and as circles for the row arrows, step numbers and the floating text circle. Two intermediate radii exist as one-offs (the Facebook row at 20px, the sent-fallback panel at 16px) and are not system steps. Nothing has a visible border at rest except the ghost button's outline, the copy button's 2px Ink outline and the hairline rules between service rows. Inputs and chips carry a 2px transparent border so hover and focus can colour it without shifting layout.

## Components

### Header
Quiet paper bar, wordmark left, number right. 64px tall on phones, 76px from 760px. The wordmark stacks "Richmond" in Cal Sans 21px (24px desktop) over a small uppercase system sub-line in Soft. The phone link is Cal Sans 17px (20px desktop) with a Yellow Ink phone glyph; on pointer hover the text turns Yellow Ink. Both are 44px+ tap targets. There is no nav menu and no call button in the hero; the number lives here.

### Hero
Deep green with texture, the client's job photo, and four things only: an eyebrow, the H1, one promise line (bold phrase in On Dark), and at most two buttons (primary "Text photos for an estimate" with a chat glyph, ghost "Fill out the estimate form"). Buttons stack full-width on phones with 12px between and sit side by side from 760px. The photo is preloaded per breakpoint (`hero-strip.webp` under 760px, `hero-wide.webp` above) and carries empty alt because the H1 and promise carry the meaning.

### Eyebrow (owner-chosen exception)
A small label pill, not a button: system 500 14px, 9px 14px padding, a 7px Equipment Yellow dot, on 6% Ink tint over light or 12% white over dark. Used above at most three headings on the page (hero, services, form), marked up as a `<p>`, never a heading. No arrow, no hover, no shadow, never a full-strength yellow fill. Impeccable flags eyebrows by default; Ellie chose LPMR-style pills on 2026-10-19 and this bounded form is the house exception.

### Buttons
- **Shape:** full pill (999px), 56px tall, 0 26px padding, Cal Sans 18px, 10px gap to a 20px glyph, 2px border.
- **Primary:** Equipment Yellow fill and border, Ink text. Hover (pointer only) Bright Yellow. Inside the white form card it is full width and also gains a 2px Fence Green outline on hover and focus, since yellow-on-white needs the extra edge.
- **Ghost:** transparent, On Dark text, 2px border at 75% On Dark. Hover: full white border and a 10% white wash. Dark grounds only.
- **Copy:** 44px pill, 2px Ink outline, transparent, Cal Sans 16px; hover adds the Fence Green outline. Lives only in the sent fallback.
- **Active:** every `.btn` scales to 0.98 over 120ms.
- **Focus:** 3px outline at 3px offset; Fence Green on light, Equipment Yellow on dark bands, the hero and the footer.

### Cards / Containers (who cards)
- **Corner Style:** 24px.
- **Background:** Card White on paper.
- **Shadow Strategy:** none (Tone-Not-Shadow).
- **Border:** none.
- **Internal Padding:** 24px; Title H3 24px, body 8px below. One column with 16px gap on phones, two columns with 24px gap from 760px.

### Service rows
Each row is a full-width text link on the fence-green band: Cal Sans row size in On Dark, 72px minimum height, 12px vertical padding, hairline `rgba(255,255,255,.14)` rules above each and below the last (and below the last of each column at 1024px). At the right is a 44px circle with an 18px arrow on 10% white. **Only the arrow changes** on hover: it fills Equipment Yellow with an Ink arrow over 200ms; the row itself gets no background, underline, outline or shadow. Keyboard focus moves to the arrow too: yellow fill plus a 3px yellow outline. On phones a tap opens a pre-written text; on pointer devices (JS) a click ticks the matching chip, scrolls to the form and focuses the location field, and the note below the list changes to "Click a job to start an estimate for it."

### Facebook row
A single fence-green pill-ish slab (20px radius) on paper, 76px min height, max 760px wide: a 28px yellow Facebook mark, Cal Sans label in On Dark, and the same 44px arrow circle at the right, which is the only thing that changes on hover or focus, exactly like the service rows.

### Work photo
The one job photo in a 24px-radius clip with a Field Mist placeholder fill, max 760px wide, lazy-loaded with a srcset. On 1024px+ it spans both grid rows on the left.

### Steps
An ordered list on deep green. Each step is a 48px Equipment Yellow circle with an Ink Cal Sans 20px numeral (CSS counter), 16px gap to a Cal Sans step heading in On Dark and a system body line in On Dark Soft. Stacked with 24px gaps on phones; three columns with 40px gaps from 1024px.

### Inputs / Fields
- **Form card:** Card White, 24px radius, `clamp(20px, 5vw, 32px)` padding, 20px between fields, max 600px.
- **Labels:** Cal Sans 17px Ink; optional hints in system 14px Soft in parentheses.
- **Text fields:** Field Mist fill, 10px radius, 2px transparent border, 13px 14px padding, 52px min height (textarea 120px, vertical resize), 16px system text in Ink, Soft placeholder, Fence Green caret.
- **Hover / Focus:** the border turns Fence Green (no glow, no outline).
- **Error:** the field's border turns Error red and stays red while focused; a 15px Error message appears below; `aria-invalid` is set; the first bad field takes focus. Typing clears the state.

### Chips
- **Style:** visually hidden checkboxes with pill labels: Field Mist fill, 48px tall, 0 18px padding (14px at 380px and below), system 16px Ink, 2px transparent border, wrapping with 10px gaps.
- **State:** hover border Fence Green; selected is a solid Ink fill with white text; keyboard focus is a 3px Fence Green outline on the label.

### Sent fallback
After submit the page hands off to an `sms:` link; 900ms later a Field Mist panel (16px radius, 16px padding, `role="status"`) appears under the button with a bold Ink line, the composed message in a pre-wrapped 15px block, and the Copy button, whose label becomes "Copied" or "Select the text above to copy". This exists for computers and in-app browsers where no messages app opens.

### Close
Fence-green band: the H2, a 36ch On Dark Soft line, and the big phone number in Phone Display with a 0.8em yellow phone glyph; hover turns it yellow. From 1024px the number sits bottom-right of a two-column grid.

### Footer
Deep green with texture, On Dark Soft text. Business name in Cal Sans 21px On Dark, one line of what he does, then phone, email and Facebook as 44px-tall On Dark links (yellow on hover) wrapping with 6px 22px gaps. Bottom padding clears the float.

### Floating text circle (signature)
One 60px Equipment Yellow circle with a 26px Ink chat glyph, fixed 16px from the bottom-right (plus safe-area insets), with the Float lift shadow. It rests 120px below the viewport and slides up over 350ms `cubic-bezier(.2,.8,.2,1)` once the hero has scrolled away, and slides back out while the estimate form is on screen. While hidden it is `aria-hidden` and out of the tab order. Removed entirely when `CONFIG.FLOAT` is false or IntersectionObserver is missing. Never a bottom bar.

### Motion
- **Hero H1 bounce-in (owner-chosen exception):** JS splits the H1 into letters inside no-wrap word spans (keeping the accent span), each sliding from `translateX(50px)` and 0 opacity to rest over 1s `cubic-bezier(.34,1.56,.64,1)`, 20ms apart. The H1 gets an `aria-label` and the letters are `aria-hidden`; when the last letter lands the original HTML is restored. Hero H1 only.
- **Fade-up:** `.rise` elements that start below the first screen get `.below` (0 opacity, 12px down) and ease in over 400ms when they enter (8% bottom root margin). Anything already on the first screen is never hidden.
- **State transitions:** 200ms colour transitions on buttons and arrows, 150ms on fields and chips, 120ms button press.
- **No JS:** the H1 is plain text, every `.rise` element is visible at rest, the float stays offscreen (it only shows via JS), and the service rows remain plain `sms:` links.
- **Reduced motion:** the H1 is never split, the fade-up never hides anything, smooth scrolling is off, and button, float and fade transitions are removed.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands light and dark (paper, fence green, deep green) so each section boundary is obvious.
- **Do** use Equipment Yellow as a fill with Ink text on it, and switch to Yellow Ink (#805c00) whenever yellow must be text or a glyph on paper or white.
- **Do** set every heading, button, row, field label and phone number in Cal Sans at 400, and running text in the system stack at 16/1.7.
- **Do** keep shapes to the three radii: 10px fields, 24px cards, full pills and circles for everything tappable or label-like.
- **Do** put fields and chips on the Field Mist fill with a 2px transparent border that turns Fence Green on hover and focus.
- **Do** make service-style links change only their arrow circle on hover and focus.
- **Do** keep focus visible: 3px outline at 3px offset, Fence Green on light, Equipment Yellow on dark bands, the hero and the footer.
- **Do** keep everything visible without JS and with reduced motion; motion only ever hides content that JS will reveal.
- **Do** limit eyebrows to a few key headings, as quiet `<p>` pills with a yellow dot.

### Don't:
- **Don't** put white text on Equipment Yellow, or Equipment Yellow text on paper or white.
- **Don't** add a second warm accent or a third green; the palette is paper, two greens, one yellow.
- **Don't** add shadows to cards, rows, buttons or fields; the floating text circle is the only lifted element.
- **Don't** give eyebrows an arrow, hover state, shadow or full yellow fill, or let them become headings or appear on every section.
- **Don't** bounce-in any heading other than the hero H1, and don't add motion beyond the bounce-in, the one 12px fade-up and short state transitions.
- **Don't** put the diagonal texture on paper or fence green, or raise it above about 4% white.
- **Don't** add a hover background, underline or outline to a whole service row or the Facebook row.
- **Don't** replace the floating text circle with a sticky bottom bar or add a second floating control.
- **Don't** bold Cal Sans or load another webfont or weight.
