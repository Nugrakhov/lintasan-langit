# Lintasan Langit — Sky Track Fortune

> Pick a date. Read the sky. Smile. A playful zodiac fortune for horse-racing fans — deterministic, mobile-first, single file.

![single-file](https://img.shields.io/badge/single--file-index.html-gold) ![no-deps](https://img.shields.io/badge/deps-none-brightgreen) ![mobile](https://img.shields.io/badge/mobile-first-yes-blue) ![lang](https://img.shields.io/badge/lang-ID_%2B_EN-orange) ![license](https://img.shields.io/badge/fun-entertainment_only-purple)

**Live demo:** Settings → Pages → Deploy from branch → `main` / root → open `https://<user>.github.io/<repo>/`

---

## What is this?

Enter your birth date, pick a race day, and the stars hand you a fortune slip: **5 BOX numbers + 1 glowing Anchor**, lucky color, star bet, luck score, and a dramatic-funny two-line reading. Same inputs always give the same stars. Download the slip as an elegant PNG and share it.

## Highlights

| | |
|---|---|
| Date + zodiac | Birth picker with auto zodiac, saved locally (`ll-lahir`) |
| Real race inputs | Race day (defaults today), JRA / NAR / INT segments, per-segment courses, R1–R12, field 5–18, optional horse names |
| Deterministic | `xmur3 + mulberry32` seed `birth\|day\|segment\|course\|raceno\|total`; Anchor on its own `seed\|jangkar` stream |
| Fortune card | Number balls, Anchor glow, lucky-color dot, animated score bar |
| PNG slip | 1080×1350 canvas: gold frame, glow, glass panel, quote block |
| Bilingual | ID default + EN toggle, persisted (`ll-lang`), same-seed re-render |
| Honest | Banner everywhere: pure entertainment, not betting advice |

## Try it in 10 seconds

```bash
# no install, no build
npx -y serve ./
# or just double-click index.html
```

1. Pick birth date → zodiac appears
2. Pick segment, course, race, field size
3. Hit **Buka Ramalan Langit** → screenshot or **Unduh Gambar Slip**

## Privacy

Birth date never leaves the browser. Clear site data to wipe `ll-lahir` / `ll-lang`.

> [!WARNING]
> Pure entertainment — not betting or financial advice.
