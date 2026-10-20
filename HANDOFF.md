# Richmond Equipment Rental LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/richmondEquipmentRental/ · **Repo:** https://github.com/10elizabethbell/richmondEquipmentRental · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, Facebook group "CONTRACTORS NJ/PA Conncted") · **Revamped:** 2026-10-19 to the calm band style

## Revamp 2026-10-19: what changed
The business hasn't been contacted, so the whole site was rebuilt under the new house default (`calm-photo-style.md`, copied from the DPG reference build). Facts, the work photo and all contact wiring carried over unchanged.
- **Look:** the "job site / underground soil" world is gone. Now paper, fence-green and deep-green bands (faint diagonal texture on the deep ones), equipment yellow as the one accent (fills only; #805c00 when it's text on light), Cal Sans headings, pill buttons, 24px cards, eyebrow pills on the hero, services and form.
- **Hero:** the drag-to-dig canvas dirt bank is removed (it's in git history at `d66e0e1`, see Ideas). The hero is now his graded-lot photo under a deep-green overlay: on phones it's a wide strip along the hero's bottom edge (fence, both machines, the laser), so the photo keeps its shape and the words sit on plain deep green; on tablet/desktop it fills the band, darkest behind the words. Measured contrast behind the hero text: 6.8:1+ white, 4.6:1+ soft text, 360–1920px.
- **H1:** "Dirty work, done right in the Poconos." (was "Let me handle the dirty work."), so the place is in the H1. It bounces in letter by letter, then restores the plain heading. Eyebrow: "For homeowners and contractors".
- **Motion:** bounce-in on the hero H1, a 12px fade-up on everything below the first screen, nothing else. Reduced motion and no-JS show everything at once.
- **Floating text circle** (bottom right, `CONFIG.FLOAT`): appears after the hero, hides while the estimate form is on screen, opens the same pre-filled text as the hero button.
- **Structure:** header (wordmark, tap-to-call number top right) → hero → "Big job or part of one." (Homeowners / Contractors cards) → services on green (6 rows, each a pre-filled text; only the arrow lights on hover) → Recent work (the photo, then a big "Click to see more of my work." Facebook row) → How estimates work (his 3-step process + "I work in the Poconos, Pennsylvania.") → estimate form → close ("Have a project coming up?" + big number) → footer (name, line, phone, email, Facebook).
- **Form:** name is now optional; location and description required, with inline errors that keep their red edge while focused. Fields use their own fill (#e5eae3) on the white card. Submits to a pre-filled text; after a moment the written message shows with "Copy message" and the number for computers.
- **Favicon and touch icon** redone in the new palette (yellow Cal Sans "R" on fence green, `img/favicon.png`, `img/apple-touch-icon.png`).
- **On computers** (fine pointer + hover) a service row doesn't try to open a text; it ticks the matching job in the estimate form and jumps there, and the note under the rows says "Click a job to start an estimate for it." Phones keep the direct pre-filled text.
- **Impeccable pass** (every mode except live, plus the finish reviewer) applied: yellow focus rings on dark bands (Facebook row, floating circle), "in the Poconos." kept on one line, no stranded words, duplicate form lede removed, close line in first person ("Call or text me."), hero secondary button now "Fill out the estimate form", sideways-phone hero fits its buttons on screen, desktop hero image preloaded, copy button label resets, the invented "Free estimate" eyebrow became "Estimates by text".
- Hero buttons: "Text photos for an estimate" (yellow) and outlined "Fill out the estimate form". The first was shortened from "Text me photos for an estimate" so it stays on one line at 360px.

- **Docs:** `DESIGN.md` and `.impeccable/design.json` rewritten from the new page; `PRODUCT.md` updated (Cal Sans, calm look). The detector's diagonal-stripes finding is ignored for `index.html` (house rule) in `.impeccable/config.json`.
- **Live check:** GitHub Pages built commit `8743841` and the live page serves the revamp (checked 2026-10-19). Call Sheet already pointed at the live URL (script reported UNCHANGED).

## Assumptions I made
- **First person "I"**: he signs the post "Steve" and writes "Send me pictures".
- **Colors**: no logo or brand exists. The calm style's navy roles are the construction-fence green from his photo (#1f4a3c / deep #10271f); the accent is the Wacker Neuson equipment yellow (#f2b705).
- **H1** adapts the flyer tagline ("LET US HANDLE THE DIRTY WORK", OCR) with the caption's "in the Poconos".
- **Owner-voice copy I wrote** (not from the brief): the hero promise ("I treat your property like it's my own and leave it ready for what comes next."), the Homeowners and Contractors lines, "Big job or part of one.", step hints ("A straight answer on what the job takes", "Compact equipment fits through gates and side yards"). Check these with Steve, especially the two operational claims: "keep the machines off what stays, and clean up before I go" and "Compact equipment fits through gates and side yards" (the brief only says "tight-access work with compact equipment").
- **Facebook link** goes to Steve's personal profile (no business page exists).
- **Favicon / touch icon**: no logo, so it's an "R" in equipment yellow on fence green.
- The same photo appears twice (hero strip and Recent work): it's the only one there is.

## Placeholders and gaps
- **Flyer facts left off the page** because the flyer image is behind a Facebook login and couldn't be checked: PA HIC #PA230262, NY 2138246-DCWP, Staten Island coverage, and the extra flyer services (drainage, small jobs welcome, subcontract/overflow work, one-day jobs, material moving).
- **Only one work photo.** No before/afters, no logo, no reviews, no hours, no prices, no Google Maps listing.

## Questions for the owner
- Can you confirm the license numbers and that you cover Staten Island too?
- Any before/after photos? (a driveway tear-out or trench would fit a slider well)
- Do you want hours on the page, or is "text me anytime" the answer?
- Is there a business Facebook page coming, or should the link stay on your profile?
- Which jobs do you want more of? That decides the service order.

## Ideas not built (yours to pick)
- **Opt-in signature motion (runner-up world):** the original drag-to-dig dirt bank (excavator bucket that digs, carries, dumps and grades to a laser line on its own). Full code at commit `d66e0e1`; it could return as a band below the hero rather than the hero itself. Other trade worlds: concrete breakout (a slab that cracks under taps), a grade-laser line sweeping across the page, gravel spread under the finger.
- Licenses as a quiet trust line once verified; Staten Island in "I work in…" once confirmed.
- Before/after slider module when photos come in; work photo cards (4:5) once there are 3+.
- Contractor-specific pre-filled text ("I need help with part of a job: …").
- **Impeccable findings kept by house rule** (Ellie's calm-style choices): eyebrow pills (craft floor bans them), the per-element `.rise` fade-up, the H1 bounce-in's overshoot curve, the diagonal band texture (detector: repeating-stripes-gradient), Cal Sans, the floating text circle. Also kept: "Click to see more of my work." wording (finishing rule) and the phone number in both the close and the footer (finishing rules allow it there; a strict reading of once-per-screen would drop the footer link).
- Make the header sticky with the kit's shadow-on-scroll (not built; DPG's header isn't sticky either).
- On Windows computers the hero "Text photos" button and the floating circle open `sms:`, which does nothing there; the number top right covers it. They could send desktop visitors to the form like the service rows do.

## Not verified
- Real-device touch and the real SMS handoff with pre-filled body on iOS, Android and inside Facebook's in-app browser.
- Cal Sans loads from Google Fonts; on a very slow connection the headings show in the fallback first.
