# 🗄️ OIBSIP

### Oasis Infobyte Summer Internship Program
**Track:** Web Development & Designing — Level 2
**Intern:** Marium Rehan Baig

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

---

## 📖 About

This repository holds all four task submissions for the Oasis Infobyte SIP, Web Development & Designing track — **Level 2**, fully completed. Each task lives in its own folder with its own README covering objective, features, and how to run it.

## ✅ Progress

| # | Task | Status | Folder | Live Demo |
|---|------|--------|--------|-----------|
| 1 | Calculator | ✅ Done | [`WebDev-L2-Calculator`](./WebDev-L2-Calculator) | [View](https://marium230-pixel.github.io/OIBSIP/WebDev-L2-Calculator/) |
| 2 | Tribute Page | ✅ Done | [`WebDev-L2-TributePage`](./WebDev-L2-TributePage) | [View](https://marium230-pixel.github.io/OIBSIP/WebDev-L2-TributePage/) |
| 3 | To-Do Web App | ✅ Done | [`WebDev-L2-TodoApp`](./WebDev-L2-TodoApp) | [View](https://marium230-pixel.github.io/OIBSIP/WebDev-L2-TodoApp/) |
| 4 | Login Authentication System | ✅ Done | [`WebDev-L2-LoginAuth`](./WebDev-L2-LoginAuth) | [View](https://login-auth-app.bonto.run/login.html) |

## 🧱 Tech Stack & Project Details

<table>
<tr>
<td valign="top" width="25%">

**🧮 Calculator**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

A dark instrument-panel calculator with a monospace readout instead of a stock light UI. Handles chained operations (`5 + 3 × 2`), catches division-by-zero with an on-screen message instead of crashing, and supports full keyboard input as a bonus. Every button is wired via `addEventListener` — no inline `onclick`.

**Highlights:** CSS Grid layout · operator chaining · keyboard support · percent key

</td>
<td valign="top" width="25%">

**🕯️ Tribute Page**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

A tribute to Ada Lovelace, the first person to publish an algorithm intended for a machine. Ink-and-parchment section design with brass/wine accents, a punch-card motif on the timeline (referencing the Jacquard loom that inspired the Analytical Engine), four original biography paragraphs, and a real 1843 quote from her own published Notes.

**Highlights:** original written biography · 5-point life timeline · styled quote block · public-domain portrait

</td>
<td valign="top" width="25%">

**✅ To-Do App**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

A task manager with rust and oxidized-steel accents that splits work into Pending and Completed lists. Supports inline editing, permanent delete, live task counters, and per-task timestamps for both creation and completion. Tasks persist across refreshes via `localStorage` — no login required.

**Highlights:** inline edit · localStorage persistence · timestamped tasks · empty-state messaging

</td>
<td valign="top" width="25%">

**🔐 Login Auth**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)

A full-stack, vault-themed auth system — the only task-level backend in this repo. Passwords are hashed with `bcrypt` before ever touching the database; sessions are server-side via HTTP-only cookies, not `localStorage`, so the dashboard route genuinely can't be bypassed by editing dev tools. Login failures return one identical, generic error regardless of which field was wrong.

**Highlights:** bcrypt password hashing · server-side sessions · protected dashboard route · duplicate-email checking

</td>
</tr>
</table>

## 📂 Structure

```
OIBSIP/
├── WebDev-L2-Calculator/
│   ├── index.html
│   └── README.md
├── WebDev-L2-TributePage/
│   ├── index.html
│   ├── portrait.jpg
│   └── README.md
├── WebDev-L2-TodoApp/
│   ├── index.html
│   └── README.md
└── WebDev-L2-LoginAuth/
    ├── server.js
    ├── package.json
    ├── public/
    ├── data/
    └── README.md
```

## 🚀 Running Each Task

**Static tasks (Calculator, Tribute Page, To-Do App):** open `index.html` directly in any browser — no install, no build step.

**Login Auth System (full-stack):**
```bash
cd WebDev-L2-LoginAuth
npm install
npm start
```
Then visit `http://localhost:3000`.

## 🔗 Connect

More of my work on [GitHub](https://github.com/marium230-pixel).

---

*#oasisinfobyte #webdevelopment #internship*
