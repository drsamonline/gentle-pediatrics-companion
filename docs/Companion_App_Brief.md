# Gentle Pediatrics — Companion App: Design & Safety Brief

A phone app for a parent at the cot side, built from the book. This file says
what it does, how it was redesigned after the first version, and what still
stands between the prototype and a public release.

## Files

```
Gentle_Pediatrics_Companion.html   the app (open in any browser; works offline)
manifest.webmanifest               PWA manifest (installable to home screen)
sw.js                              service worker (offline caching)
icon-192.png, icon-512.png         app icons
Companion_App_Brief.md             this file
```

Open the HTML on a phone, tap **Add to Home Screen**, and it runs full screen and
offline with no account.

## What changed from the first version (and why)

The first build put a mandatory, eight-item emergency checklist in front of
everything. Those items were so broad — "unusually sleepy", for instance — that
any parent of a sick child would tick one, so the app funnelled almost everyone
to "call emergency" and never reached a remedy. That was a bad design, and it
made the app useless for the everyday case it was meant to help with.

The redesign inverts it:

- **The remedies are now the main experience.** The home screen is nine symptom
  tiles; tap one and the remedy options are visible immediately — no gate, no
  checklist to clear first.
- **The emergency check is a tight, per-symptom strip** at the top of each
  screen, listing only the two or three signs that are genuine emergencies for
  *that* situation, with a single "Yes — one of these applies" button that opens
  the full red-flag page. It cannot be missed, but ordinary cases pass it
  without doing anything.
- **Two taps to a remedy:** tap the symptom, tap the description that fits. You
  then get the remedy card — the key picture, the modalities, the dose from the
  book, a "reassess" box, and a "stop and get help if" list.

## What it does now

1. **Home** — nine situations: fever, cough, earache, belly pain, teething and
   sleep, diarrhoea, rash, wheeze, bump and burn.
2. **Situation screen** — the emergency strip, then the remedy options for that
   picture, each labelled with the one-line keynote that separates it.
3. **Remedy card** — key picture, modalities (better/worse), the book's dose, a
   reassess note, and when to escalate.
4. **Remedies** (header) — an index of all twenty remedies with the one-line
   picture for each.
5. **Red flags** (header) — the full emergency list and the glass test.
6. **About** — how to use it, what it will not do, and the honest limits.

## The safety model

- **Triage is visible, not hidden, but it no longer blocks the common case.** The
  emergency signs sit in a red strip at the top of every symptom screen, and the
  one-tap emergency button is always there.
- **It never diagnoses.** The remedy panel is labelled "gentle orientation —
  confirm with a clinician", and every screen carries the footer: *not a
  diagnosis; homeopathy never replaces emergency care, oxygen, IV fluids,
  antibiotics or surgery.*
- **The dose is attributed and bounded** — quoted from the book, with the rule
  never to give anything by mouth to a drowsy or struggling child.
- **Offline and private** — no account, no analytics, nothing stored or sent.
- **The limits are stated plainly**, including that the evidence base is
  contested and that there are no homeopathic vaccines.

## What a real release still needs

1. **Clinical sign-off.** Every red flag, keynote and dose must be reviewed and
   signed off by a licensed clinician (ideally a paediatrician) and versioned
   against the book edition.
2. **Regulatory check.** Software making diagnostic or therapeutic claims can be
   regulated as a medical device (in India, CDSCO's rules and the SaMD guidance;
   app-store health-claim policies elsewhere). The safe position is *educational
   / wellness*, making no diagnostic claim — which is how this is written.
3. **Emergency numbers per region** (the app defaults to 108 / 112).
4. **Localisation** into Hindi and the other languages of the book.
5. **Accessibility** — screen-reader labels, larger targets, higher contrast.
6. **Parent testing**, especially that they notice the red-flag strip and do not
   feel diagnosed.
7. **Hosting over HTTPS** so the service worker can install.
8. **Consider dropping the dose numbers** in a public build, leaving only "give
   it as your clinician directs".

## Possible next steps

- A side-by-side "look-alike" comparison for the pairs the book flags (Chamomilla
  vs Cina, Pulsatilla vs Silica), mirroring Chapter Eight.
- A short red-flag practice quiz.
- Deep links from each screen back to the matching chapter of the book.
- A "clinic handover" screen: a one-page summary of what was observed, when it
  started, and what has been given, to show a doctor.

## Honest limits of this prototype

- A single-file demonstration, not a validated or regulated product.
- The remedy keynotes are condensed from the book and not independently
  re-verified for this app.
- It covers the nine acute situations in the book — it is not a general symptom
  checker and must not be used as one.
