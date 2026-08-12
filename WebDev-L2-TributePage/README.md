# 🕯️ Tribute Page — Ada Lovelace

A tribute page built around the person history calls the first computer programmer — a Victorian mathematician who described an algorithm for a machine that wouldn't exist for another hundred years.

Built for the **Oasis Infobyte SIP — Web Development & Designing, Level 2**.

`HTML5` `CSS3` `No-Framework`

🔗 **Repository:** [github.com/marium230-pixel/OIBSIP/tree/main/WebDev-L2-TributePage](https://github.com/marium230-pixel/OIBSIP/tree/main/WebDev-L2-TributePage)
🌐 **Live Demo:** [marium230-pixel.github.io/OIBSIP/WebDev-L2-TributePage](https://marium230-pixel.github.io/OIBSIP/WebDev-L2-TributePage/)

---

## 📌 Task Objective

Design and build a tribute page for a historical figure, scientist, artist, or public figure — original written content, a real portrait, a timeline of key achievements, and a distinct visual identity, not a generic Wikipedia reskin.

## 💡 Why Ada Lovelace

She's the person most computer science curricula trace the discipline back to: in 1843, she wrote "Note G," a step-by-step method for Charles Babbage's unbuilt Analytical Engine to compute Bernoulli numbers — recognized today as the first algorithm ever written for a machine. As a CS student, that felt like the right person to build this around.

## 🎨 Design Concept

The page borrows its visual language from Lovelace's own world rather than a generic template:

- **Ink & parchment** — sections alternate between a deep engine-iron ink background and a warm parchment tone, echoing bound ledger pages next to a mechanical instrument panel.
- **Brass & wine accents** — brass gold for structural marks (mirroring Victorian engineering fittings), deep wine for the quote block and the biography's drop cap.
- **Typography** — Playfair Display for headlines (period-appropriate serif elegance), EB Garamond for body copy, IBM Plex Mono for dates, labels, and the algorithm-flavored details — a nod to her being the first person to write instructions *for* a machine.
- **Signature element** — the timeline opens with a punch-card strip of filled/empty cells, referencing the Jacquard loom that directly inspired the Analytical Engine's design, and each timeline node is a rotated square "card" rather than a generic circle.

## ✨ Features

- Full-bleed hero with a subject tagline and an embedded portrait (Chalon watercolour, 1840 — public domain, sourced from Wikimedia Commons)
- Biography section: four original paragraphs covering her upbringing, mentors, meeting Babbage, and her published Notes
- Timeline of five key life events, from birth to her death at 36
- A distinctly styled quote block featuring a real line from her own 1843 Notes
- Two clearly different section background colours (ink vs. parchment), per the task's colour requirement
- Two paired font families plus a monospace utility face, per the task's typography requirement
- Fully responsive — hero and timeline both restack cleanly on mobile

## 🛠️ Tech Stack

| Layer | Choice |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 — CSS Grid + Flexbox, custom properties for theming |
| Image | Wikimedia Commons (public domain) |
| Fonts | Playfair Display, EB Garamond, IBM Plex Mono (Google Fonts) |

## 📂 Project Structure

```
WebDev-L2-TributePage/
├── index.html      # Structure, styles, and content — single-file build
└── README.md
```

## 🚀 Running It Locally

No install, no build step, no dependencies.

```bash
git clone https://github.com/marium230-pixel/OIBSIP.git
cd OIBSIP/WebDev-L2-TributePage
open index.html    # or just double-click it
```

## 👩‍⚖️ Notes for Evaluators

- Biography content is original writing, paraphrased from historical research — not copied from any single source.
- The one direct quotation used is Lovelace's own 1843 words from her published Notes, now in the public domain.
- Portrait is sourced from Wikimedia Commons under public domain licensing (painted 1840, well past any copyright term).

## 🔮 Possible Next Steps

- Scroll-triggered reveal animation on the timeline
- A second tab for her personal letters/correspondence excerpts
- Light/dark palette toggle

---

*#oasisinfobyte #webdevelopment #internship*
