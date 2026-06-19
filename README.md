# ✨ Pangeya Essay Platform

A modern, hi-tech web app for **IELTS Writing practice**. Students write, save and
print essays; teachers leave feedback with a secret key; and **PangeyaAI** — a built‑in
AI assistant — helps with structure, samples and band‑level feedback.

> Single‑file app (`index.html`). No build step. Hosted on GitHub Pages, data in
> Firebase Firestore. Styled in the **pangea8** brand language (dark neon‑mint, Space Grotesk, animated spark).

---

## ✦ Features

### ✍️ Writing Studio
- **Task switch** — IELTS *Task 2 (40 min)* / *Task 1 (20 min)* with the right structure hint.
- **Exam timer** — start / pause / reset, turns amber in the last 5 minutes and alerts when time is up.
- **Live word ring** — counts words against the target (250 / 150) and turns green when reached.
- **Auto‑save** — every keystroke is saved to your browser (survives refresh / lost connection) and clears after you submit.
- **💡 Structure** — band‑9 outline for the selected task.

### 🤖 PangeyaAI
- In‑page AI assistant for IELTS Academic & General Writing.
- Suggestion chips (Task 2 structure, Band 9 sample, cohesion, linking words).
- Per‑essay **AI Feedback** with an estimated band and improvement notes.
- Chat‑credit system (type `please` three times in a row for 13 extra messages).

### 📋 Essay Dashboard
- Responsive **card grid** of all submitted essays.
- **Status badges** — `✓ Reviewed`, `✦ AI checked`, or `Submitted`.
- Word count, date, expandable **Teacher Feedback** / **AI Feedback** panels.
- Quick actions: Edit · Get AI Feedback · Download PDF (Delete & feedback tools in teacher mode).

### 🧑‍🏫 Teacher mode
- Enter the secret teacher key to unlock editing, highlighting, underlining, strike‑through and feedback.

### 🎨 Themes & extras
- **Mint / Light / Black** themes (pangea8 dark-mint by default).
- Export any essay to **PDF** (jsPDF).
- Glassmorphic, animated, mobile‑friendly UI.

---

## 🛠 Tech stack

| Layer        | Tech                                            |
|--------------|-------------------------------------------------|
| Frontend     | HTML, CSS, vanilla JavaScript (single file)     |
| Database     | Firebase **Firestore**                          |
| AI backend   | PangeyaAI API (Vercel)                           |
| PDF export   | jsPDF                                            |
| Hosting      | GitHub Pages                                     |

---

## 🚀 Run / deploy

It's a static single‑file app — just serve `index.html`.

**GitHub Pages**
1. Put `index.html` (and optional `donation_qr.png`) in the repo root.
2. **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / root.**
3. Open `https://<username>.github.io/<repo>/`.

**Local**
```bash
# any static server, e.g.
python3 -m http.server 8000
# then open http://localhost:8000
```

> **Firebase note:** Firestore access is controlled by Security Rules (not by domain),
> and all GitHub Pages sites for a user share the same `*.github.io` domain — so existing
> essays load on any repo under your account without extra configuration.

---

## 📖 How to use

**Students**
1. Enter your name and write your essay (timer + word ring help you stay on target).
2. **Submit** to save it to the cloud, or **Download PDF**.
3. Ask **PangeyaAI** for help, or click **Get AI Feedback** on a saved essay.

**Teachers**
1. Click **Teacher Login**, enter the secret key.
2. Edit essays, highlight / underline / strike text, and add feedback.
3. The key is confidential — contact the developer to request it.

---

## 👤 Author

**Maqsudjon Polatov** — developer of the Pangeya Essay Platform, PangeyaAI, and more.

If you'd like to support development, see the in‑app **Author Info** panel.

---

*Built with care for IELTS learners. 🌱*
