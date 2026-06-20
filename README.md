# Pangeya — IELTS Writing Lab

A focused, single-file IELTS writing workspace with a Nothing-inspired interface — monochrome, dot-matrix type, a red accent, and subtle hi-tech motion. Write timed essays, save them to the cloud, get teacher feedback and on-demand AI scoring, and export clean branded PDFs.

**Live:** https://maqsudjon-cell.github.io/pangeya-essay-platform-/index-14.html

---

## Features

- **Timed composing** — Task 1 (20 min / 150 words) and Task 2 (40 min / 250 words) with a live timer that pulses and beeps in the final minute, plus a colour-coded word-count ring (amber under target, green once you hit it, with an "X to go" hint).
- **Focus mode** — hides everything but the editor, timer, and word count for a distraction-free, exam-like view (Esc to exit).
- **Cloud archive** — essays save to Firebase and render instantly from an in-memory cache; search by name or keyword with no re-fetching.
- **Pangeya AI** — a floating examiner you can open from anywhere. Ask about structure, vocabulary, sample answers, and band scores.
- **Per-essay AI feedback** — request an estimated band score and notes on any archived essay; the result stays collapsed until you open it.
- **Teacher mode** — a key unlocks editing, deleting, written feedback (✔ strengths / ✘ fixes), and personal gift messages per student.
- **Branded PDF export** — every essay exports as a clean PDF with the Pangeya mark, candidate details, word count, and any teacher feedback. Designed to look sharp in both colour and greyscale.
- **Fair-exam editor** — spellcheck, autocorrect, and grammar underlines are disabled so students write without hints.
- **Light / dark themes**, draft autosave, and a built-in how-to guide.

## Tech

- Single static `index.html` — no build step.
- **Firebase Firestore** for essays and gift messages.
- A small **Vercel** API (`pangeya-ai`) proxies chat and essay feedback to OpenAI.
- **jsPDF** for exports.
- Vanilla JavaScript, no framework.

## Structure

```
index.html        # the entire app (HTML + CSS + JS)
```

## Brand

Part of the **pangea8** ecosystem. Tashkent.
