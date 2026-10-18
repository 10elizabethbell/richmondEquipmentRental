# Richmond Equipment Rental LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/richmondEquipmentRental/ · **Repo:** https://github.com/10elizabethbell/richmondEquipmentRental · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, Facebook group "CONTRACTORS NJ/PA Conncted")

## What's built
- One page, `index.html` (single file, inline CSS/JS, system fonts), photo and icons in `img/`.
- World: an active job site. Construction-fence green (from the fence in his photo) over soil; equipment yellow on the buttons; grade-laser red for the laser line and the form's hover/focus outlines. Scrolling goes "underground": services and the estimate form sit on soil-colored layers with organic seams.
- Signature element: a canvas dirt bank across the bottom of the hero (behind the headline on desktop, with a spoil pile on the right). An excavator bucket follows finger or mouse: drag into the soil to dig, what doesn't fit gets shoved ahead, hold it still in the air to tip and dump. Soil slumps to an angle of repose and grains fly and land. The bucket has a stick, a hydraulic cylinder and a shadow on the soil; it digs teeth-down, curls to carry and tips to dump. Left alone for ~2.6s it grades the high spots down to the beam of a tripod rotary laser (like the one in his photo), drops the spoil in the low spots, and once it's level digs a trench and heaps it beside, so there's always work. Soil is conserved (nothing appears or vanishes). A second dirt bank buries the bottom edge of the work photo; it's still until you drag in it, and vertical swipes scroll there. Tunables are in `TUNE` at the top of the dirt script.
- Sections: header (name, "Poconos, PA", tap-to-call number top-right) → hero ("Let me handle the dirty work.", promise, "Text me photos for an estimate" + outlined "Estimate form") → What I do (6 service rows, each opens a text naming that job) + Homeowners / Contractors → How estimates work (his own process: pictures, location, description) + where I work + estimate form → Recent work (his photo) → "Click to see more of my work." Facebook button → close ("Have a project coming up?", verbatim) → footer (name, phone, email, Facebook).
- Contact: everything goes to 917-525-7878. Service rows are real `sms:` links in the HTML (work without JS). Form validates location + description (errors announced to screen readers), then opens a pre-filled text; visitor attaches photos in their messages app. On computers that can't text, the written message stays on screen with a copy button.

## Assumptions I made
- **First person "I"**: he signs the post "Steve" and writes "Send me pictures". The flyer's "Let us handle the dirty work" became "Let me handle the dirty work."
- **Colors**: no logo or brand exists. Green from the construction fence in his photo, yellow from the Wacker Neuson / Deere equipment, red from the laser level in the same photo.
- **Owner-voice copy I wrote** (not from the brief): the hero promise ("I dig it, break it out and grade it, then leave your site clean…"), the Homeowners line ("I work it carefully, keep the machines off what stays, and clean up before I go"), and step hints ("Straight answer on what it takes", "Compact equipment fits through gates and side yards"). Check these with Steve.
- **Contractors line** is built from the caption ("need help with part of a job?") plus the flyer tagline ("so your crew can focus on the install"), which is OCR.
- **Facebook link** goes to Steve's personal profile (no business page exists). The brief flags this.
- **Favicon / home-screen icon**: no logo, so it's an "R" in equipment yellow over a dirt line on fence green.

## Placeholders and gaps
- **Flyer facts left off the page** because the flyer image is behind a Facebook login and couldn't be checked: PA HIC #PA230262, NY 2138246-DCWP, Staten Island coverage, and the extra flyer services (drainage, small jobs welcome, subcontract/overflow work, one-day jobs, material moving). Once verified, the licenses make strong trust lines near the close, and Staten Island belongs in "Where I work" (the 917 number and "Richmond" name both point to it).
- **Only one work photo** (the graded lot from the post preview, 2048px original). No before/afters, no logo, no reviews, no hours, no prices.
- No Google Maps listing.

## Questions for the owner
- Can you confirm the license numbers and that you cover Staten Island too?
- Any before/after photos? (a driveway tear-out or trench would fit a slider well)
- Do you want hours on the page, or is "text me anytime" the answer?
- Is there a business Facebook page coming, or should the link stay on your profile?
- Which jobs do you want more of? That decides the service order.

## Ideas not built (yours to pick)
- Runner-up world: **concrete breakout**: a slab across the hero that cracks under taps like a breaker hammer, chunks you can drag off.
- A "you graded it!" reward when the visitor gets the whole bank to the laser line (a puff of dust, the line turns green).
- Licenses as a quiet trust line once verified.
- Before/after slider module when photos come in.
- Contractor-specific prefilled text ("I need help with part of a job: …").

## Not verified
- Desktop "How estimates work": the left column is sticky beside the taller form to soften the empty space; a better fill (e.g. a second photo) needs more photos.
- Detector still reports one "tight leading" (1.24x) I couldn't find at runtime; left standing. Roboto "overused font" is ignored on purpose (it's only the Android fallback in the system stack).
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser): dragging in the dirt is `touch-action: none`, so that strip doesn't scroll the page by design (as on T&J).
- Real SMS handoff with the pre-filled body on iOS and Android.
- Frame rate on older phones (grain cap 500 on phones, canvas DPR capped at 1.5).
