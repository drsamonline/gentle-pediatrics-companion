<div align="center">
  <img src="banner.svg" alt="Gentle Pediatrics — Home Companion" width="100%">
</div>

<div align="center">

**A small, offline phone app for a parent at the cot side — built from the book
*Gentle Pediatrics: A Practical Homeopathic Companion* by Dr. Sohil Momin, B.H.M.S.**

[![Live app](https://img.shields.io/badge/%E2%96%B6%20OPEN%20THE%20APP-live-2ea44f
[![License](https://img.shields.io/badge/license-free%20to%20use-c46849
[![PWA](https://img.shields.io/badge/PWA-offline%20ready-425848

![Dependencies](https://img.shields.io/badge/dependencies-none-55755e
![Build](https://img.shields.io/badge/build-single%20file-6e675d
![Not a medical device](https://img.shields.io/badge/not%20a-medical%20device-b84a39
![From the book](https://img.shields.io/badge/from-Gentle%20Pediatrics-425848
![Stars](https://img.shields.io/github/stars/drsamonline/gentle-pediatrics-companion

### ▶️ [**Open the live app →**](https://drsamonline.github.io/gentle-pediatrics-companion/)

</div>

---

<div align="center">
  <img src="docs/screens.svg" alt="Three app screens: the home list of situations, a remedy card, and the remedies index" width="100%">
</div>

---

## What it does

- **Nine situations**, one tap from the home screen — fever, cough, earache,
  belly pain, teething & sleep, diarrhoea, rash, wheeze, and bump & burn.
- **A red-flag strip on every screen** — the two or three signs that are genuine
  emergencies for *that* situation, with a one-tap path to emergency help.
- **Remedy orientation** — tap the picture closest to the child and get the
  remedy card: the key picture, the modalities (better / worse), the dose from
  the book, a "reassess" note, and a "stop and get help if" list.
- **Remedies index** — all twenty remedies in the book, with the one-line picture
  that separates each.
- **Red flags page** — the full emergency list and the glass test.

Two taps gets a parent to a remedy. The emergency check is always visible, never
hidden, and never blocks the common case.

## Install it like an app

It is a Progressive Web App. Open the
**[live app](https://drsamonline.github.io/gentle-pediatrics-companion/)** on a
phone, then:

- **iPhone (Safari):** Share → *Add to Home Screen*
- **Android (Chrome):** ⋮ menu → *Add to Home screen* / *Install app*

It then runs **full screen and offline**, with no account, no analytics, and
nothing stored or sent.

## Run it locally

No build step, no dependencies. Open `index.html` in any browser, or serve the
folder:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Safety notice — please read

This app is **not a diagnosis and not a substitute for a doctor.**

- Homeopathy never replaces emergency resuscitation, oxygen, IV fluids, indicated
  antibiotics or surgery.
- There are no homeopathic vaccines.
- Homeopathy's evidence base is contested in modern clinical research.
- If the child is struggling to breathe, is drowsy or floppy, has a rash that
  does not fade under a clear glass, or is a baby under 12 weeks with any fever —
  **call your local emergency number now** (108 / 112 India · 999 UK · 911 US).
  Do not give a remedy first.
- Always confirm any remedy with a licensed clinician.

The remedy keynotes and doses are condensed from the book and are for educational
orientation only.

## Files

| File | What it is |
|---|---|
| `index.html` | the app — a single self-contained file |
| `manifest.webmanifest` | PWA manifest |
| `sw.js` | offline service worker |
| `icon.svg` | app icon |
| `banner.svg` | README banner |
| `docs/screens.svg` | README screenshots |
| `docs/Companion_App_Brief.md` | design & safety brief |

## Credits

Built from *Gentle Pediatrics: A Practical Homeopathic Companion* by
**Dr. Sohil Momin, B.H.M.S.** Clinical vignettes in the book are composite
teaching cases.

## License

**Free to use.** Copyright © 2026 Dr. Sohil Momin. Free to use, copy and share
for personal, educational and non-commercial purposes, with attribution and this
notice kept. Commercial use or resale needs written permission. See
[LICENSE](LICENSE) for the full terms and the medical disclaimer.

<div align="center">
<sub>Not a medical device · educational aid only · in an emergency, call your local emergency number.</sub>
</div>
