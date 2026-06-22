# DDIA Interactive

An interactive companion to **Martin Kleppmann's _Designing Data-Intensive Applications_** — the whole book turned into a dark-themed, clickable learning site. Every chapter is a self-contained page with tabbed sections, deep-dive cards, diagrams, a full glossary, a self-check quiz, and at least one live interactive widget. A separate category-wise **Dictionary** page covers every key term with a live search.

No build step, no dependencies — just static HTML/CSS/JS. Open `index.html` and go.

## Contents

| File | What it is |
|------|------------|
| `index.html` | Landing page — all chapters + the Dictionary, as cards |
| `chapter01.html` … `chapter12.html` | One interactive page per chapter (Parts I–III) |
| `glossary.html` | The Complete Vocabulary — 278 terms by category, with search |

Chapters:

**Part I — Foundations of Data Systems**
1. Reliable, Scalable & Maintainable Applications
2. Data Models & Query Languages
3. Storage & Retrieval
4. Encoding & Evolution

**Part II — Distributed Data**
5. Replication
6. Partitioning
7. Transactions
8. The Trouble with Distributed Systems
9. Consistency & Consensus

**Part III — Derived Data**
10. Batch Processing
11. Stream Processing
12. The Future of Data Systems

## View locally

Just open `index.html` in any browser. Everything is relative, so it works straight off the filesystem — no server needed.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `ddia-interactive`).
2. Put these files at the **root** of the repo and push:
   ```bash
   git init
   git add .
   git commit -m "DDIA interactive site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/ddia-interactive.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. Your site goes live at `https://<your-username>.github.io/ddia-interactive/` within a minute or two.

> Prefer keeping the site in a subfolder? Move these files into a `docs/` folder and choose `/docs` as the Pages source instead.

## Notes

- Built from the 2017 early-release edition (Chapters 1–11). **Chapter 12 — The Future of Data Systems** was authored from knowledge of the later retail edition to complete the book.
- This is an educational companion and paraphrases concepts in original words; it does not reproduce the book's text. All credit for the ideas belongs to Martin Kleppmann. If you find this useful, buy the book.

## License

Content is provided for personal/educational use. Add a `LICENSE` file if you intend to share or modify it publicly.
