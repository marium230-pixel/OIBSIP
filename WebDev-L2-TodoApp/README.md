# ✅ To-Do Web App

A task manager that splits pending and completed work into their own tracked lists — add, edit inline, complete, delete, and everything survives a page refresh.

Built for the **Oasis Infobyte SIP — Web Development & Designing, Level 2**.

`HTML5` `CSS3` `JavaScript` `No-Framework`

🔗 **Repository:** [github.com/marium230-pixel/OIBSIP/tree/main/WebDev-L2-TodoApp](https://github.com/marium230-pixel/OIBSIP/tree/main/WebDev-L2-TodoApp)

---

## 📌 Task Objective

Build an interactive to-do list that goes beyond a single flat list — tasks need to move between a Pending and a Completed state, support inline editing, and persist so a student doesn't lose their list on an accidental refresh.

## 💡 Approach

Tasks live in one array of objects (`{ id, text, completed, createdAt, completedAt }`) and are filtered into two rendered lists on every re-render, rather than maintaining two separate arrays that could drift out of sync. Every task gets a unique ID at creation so edit/delete/toggle actions target exactly one task regardless of list position.

Persistence uses `localStorage` — no backend, no login, so the whole thing works offline and reloads instantly.

## ✨ Features

- ➕ Add tasks via button click or Enter key
- 📥 New tasks appear immediately in the Pending list
- ✔️ Toggle-complete moves a task into the Completed list (and back)
- ✏️ Inline edit — click the pencil, edit in place, save with Enter or the checkmark
- 🗑️ Permanent delete from either list
- 🔢 Live "X pending" / "Y completed" counters
- 🕒 Timestamp on every task — when added, and when completed
- 💾 Tasks persist across refreshes via `localStorage`
- 🫙 Friendly empty-state messaging when a list has nothing in it

## 🛠️ Tech Stack

| Layer | Choice |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 — Flexbox layout, custom properties for theming |
| Logic | JavaScript (Vanilla) — DOM built via `createElement`, no template strings for user content (XSS-safe by construction) |
| Storage | Browser `localStorage` |
| Fonts | IBM Plex Mono (labels/meta), Inter (UI) |

## 🎨 Design Notes

Warm rust palette — burnt-orange (`#c1502e`) marks completed tasks and the primary Add action, paired with a muted oxidized-steel sage (`#7d8f85`) for the Pending list, sitting on a near-black warm brown base. The pairing reads like raw rust next to weathered steel rather than a generic warm/cool accent split.

## 📂 Project Structure

```
WebDev-L2-TodoApp/
├── index.html      # Structure, styles, and logic — single-file build
└── README.md
```

## 🚀 Running It Locally

No install, no build step, no dependencies.

```bash
git clone https://github.com/marium230-pixel/OIBSIP.git
cd OIBSIP/WebDev-L2-TodoApp
open index.html    # or just double-click it
```

## 👩‍⚖️ Notes for Evaluators

- Task text is inserted via `textContent`, not `innerHTML` — safe against any accidental markup typed into a task.
- Refresh the page after adding a few tasks to confirm `localStorage` persistence.
- Try editing a task and pressing `Escape` to confirm it cancels without saving.

## 🔮 Possible Next Steps

- Drag-to-reorder within a list
- Due dates with overdue highlighting
- Tags/categories with filtering

---

*#oasisinfobyte #webdevelopment #internship*
