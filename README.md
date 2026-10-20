# Gentle Pediatrics — Home Companion

A small, offline phone app for a parent at the cot side, built from the book
**Gentle Pediatrics: A Practical Homeopathic Companion** by **Dr. Sohil Momin,
B.H.M.S.**

It helps with one thing first — *does this child need emergency care right
now?* — and then offers gentle homeopathic orientation for the common acute
situations.

**Free to use.** Copyright is retained; see [LICENSE](LICENSE).

---

## What it does

- **Nine situations**, one tap from the home screen: fever, cough, earache,
  belly pain, teething & sleep, diarrhoea, rash, wheeze, and bump & burn.
- **A red-flag strip on every screen** — the two or three signs that are genuine
  emergencies for *that* situation, with a one-tap path to emergency help.
- **Remedy orientation** — tap the picture closest to the child and get the
  remedy card: the key picture, the modalities (better / worse), the dose from
  the book, a "reassess" note, and a "stop and get help if" list.
- **Remedies index** — all twenty remedies used in the book, with the one-line
  picture that separates each.
- **Red flags page** — the full emergency list and the glass test.

## Install it like an app

It is a Progressive Web App (PWA). Hosted over HTTPS (for example GitHub Pages),
open it on a phone and use **Add to Home Screen**. It then runs full screen and
**offline**, with no account, no analytics, and nothing stored or sent.

## Run it locally

No build step, no dependencies. Open `index.html` in any browser, or serve the
folder:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Safety notice — please read

This app is **not a diagnosis and not a substitute for a doctor.**

- Homeopathy never replaces emergency resuscitation, oxygen, IV fluids,
  indicated antibiotics or surgery.
- There are no homeopathic vaccines.
- Homeopathy's evidence base is contested in modern clinical research.
- If the child is struggling to breathe, is drowsy or floppy, has a rash that
  does not fade under a clear glass, or is a baby under 12 weeks with any fever
  — call your local emergency number **now** (108 / 112 in India; 999 UK;
  911 US). Do not give a remedy first.
- Always confirm any remedy with a licensed clinician.

The remedy keynotes and doses are condensed from the book and are for
educational orientation only.

## Files

```
index.html               the app (single self-contained file)
manifest.webmanifest     PWA manifest
sw.js                    offline service worker
icon.svg                 app icon
docs/Companion_App_Brief.md   design & safety brief (what it does, and what a
                              public release would still need)
```

## Credits

Built from *Gentle Pediatrics: A Practical Homeopathic Companion* by
Dr. Sohil Momin, B.H.M.S. Clinical vignettes in the book are composite teaching
cases.

## License

Free to use, copy and share for personal, educational and non-commercial
purposes, with the copyright notice kept. Commercial use or resale needs written
permission. See [LICENSE](LICENSE).
