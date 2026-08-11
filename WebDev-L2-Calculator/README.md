# 🧮 Calculator

A calculator that doesn't look like a form — dark instrument panel, monospace readout, and operators you can actually track at a glance.

Built for the **Oasis Infobyte SIP — Web Development & Designing, Level 2**.

`HTML5` `CSS3` `JavaScript` `No-Framework`

🔗 **Repository:** [github.com/marium230-pixel/OIBSIP/tree/main/WebDev-L2-Calculator](https://github.com/marium230-pixel/OIBSIP/tree/main/WebDev-L2-Calculator)

---

## 📌 Task Objective

Level 2 of the OIBSIP Web Dev track asks for a fully functional, browser-based calculator with a button interface — not just arithmetic that works, but a UI that handles the edge cases real calculators have to: chained operations, division by zero, and backspacing a wrong digit, all without ever crashing or freezing the display.

Most beginner calculator builds stop at "it computes 2+2." This one is built to survive the ways people actually type into a calculator — fast, mid-expression corrections and all.

## 💡 Approach

Every keypress is wired through `addEventListener` — zero inline `onclick` attributes, per the task's explicit requirement. State is tracked as three plain variables (current value, previous value, pending operator) rather than `eval()`-ing a raw string, which keeps division-by-zero and malformed input catchable before they ever hit the display.

Operator chaining (`5 + 3 × 2`) evaluates the pending operation the moment a new operator is pressed, so the result feeds forward automatically instead of requiring a manual equals in between.

## ✨ Features

- 🖥️ Live expression trail above a large monospace result readout
- 🔢 Full digit entry (0–9) + decimal point
- ➕➖✖️➗ All four operators, visually distinct from number keys
- 🟰 Equals — evaluates the full pending expression
- 🧹 Clear — full state reset
- ⌫ Backspace — deletes one character at a time
- 🔗 Operator chaining — no manual reset needed mid-expression
- 🚫 Division-by-zero caught with an on-screen message, never a crash
- ⌨️ **Bonus:** full keyboard support (digits, operators, Enter, Backspace, Esc)
- ➗ **Bonus:** percent (`%`) key

## 🛠️ Tech Stack

| Layer | Choice |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 — CSS Grid for the button layout, custom properties for theming |
| Logic | JavaScript (Vanilla) — no libraries, no `eval()` |
| Fonts | IBM Plex Mono (display), Inter (UI) |

## 🎨 Design Notes

Palette is deep charcoal (`#14171c`) rather than a stock light calculator UI — teal (`#4fd1c5`) marks the equals key and status indicator, warm amber (`#ff9d5c`) is reserved only for operators, so the two functional categories (compute vs. operate) are separable at a glance without reading labels.

## 📂 Project Structure

```
WebDev-L2-Calculator/
├── index.html      # Structure, styles, and logic — single-file build
└── README.md
```

## 🚀 Running It Locally

No install, no build step, no dependencies.

```bash
git clone https://github.com/marium230-pixel/OIBSIP.git
cd OIBSIP/WebDev-L2-Calculator
open index.html    # or just double-click it
```

## 👩‍⚖️ Notes for Evaluators

- All interactivity is vanilla JS with `addEventListener` — confirmed no inline `onclick` attributes anywhere in the markup.
- Division-by-zero is handled explicitly (not via NaN/Infinity leaking to the display) — try `5 ÷ 0` to see the caught error state.
- Try `5 + 3 × 2 =` to confirm chained operator handling evaluates step-by-step rather than requiring a reset between operators.

## 🔮 Possible Next Steps

- Scientific mode toggle (sin/cos/log, parentheses support)
- Calculation history panel with click-to-recall
- Theming switch (light/dark) stored per session

---

*#oasisinfobyte #webdevelopment #internship*
