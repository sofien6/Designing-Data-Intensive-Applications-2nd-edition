# DDIA 2nd Edition — Chapter Study Pages

Interactive study guides for **_Designing Data-Intensive Applications_ (2nd edition)** by Martin Kleppmann and Chris Riccomini.

Each chapter is summarized in a single, self-contained web page: key ideas, a glossary, flashcards, and a quiz.

## 🌐 Browse online, no install needed

**https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/**

This link opens the home page ([`index.html`](index.html)), which lists every available chapter as a card with a short summary. Pick one and start studying. You don't need to download, install or build anything.

> These pages are study notes meant to accompany the book, not replace it. Please buy the book to support the authors.

## Chapters

| # | Chapter | Read online |
|---|---------|-------------|
| 1 | Trade-Offs in Data Systems Architecture | [ch01-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch01-study.html) |
| 2 | Defining Nonfunctional Requirements | [ch02-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch02-study.html) |
| 3 | Data Models and Query Languages | [ch03-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch03-study.html) |
| 4 | Storage and Retrieval | [ch04-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch04-study.html) |
| 5 | Encoding and Evolution | [ch05-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch05-study.html) |
| 6 | Replication | [ch06-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch06-study.html) |
| 7 | Sharding | [ch07-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch07-study.html) |
| 8 | Transactions | [ch08-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch08-study.html) |
| 9 | The Trouble with Distributed Systems | [ch09-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch09-study.html) |
| 10 | Consistency and Consensus | [ch10-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch10-study.html) |
| 11 | Batch Processing | [ch11-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch11-study.html) |
| 12 | Stream Processing | [ch12-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch12-study.html) |
| 13 | A Philosophy of Streaming Systems | [ch13-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch13-study.html) |
| 14 | Doing the Right Thing | [ch14-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/ch14-study.html) |

More chapters will be added over time.

### Reference

| Page | What it covers | Read online |
|------|----------------|-------------|
| Glossary | The book's 61 core terms by theme, with opposites, look-alikes, flashcards and a quiz | [glossary-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/glossary-study.html) |
| Index | The book's index made searchable: concept finder, cross-chapter threads, tech catalog, aliases, and "which chapter?" drills | [index-study.html](https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/index-study.html) |

## How to use

**Online:** use the links above.

**Offline:** clone or download the repo, then open `index.html` (or any file in `study-pages/`) in a browser (double-click works):

```bash
git clone https://github.com/sofien6/Designing-Data-Intensive-Applications-2nd-edition.git
```

Suggested routine per chapter:

1. Read the chapter in the book.
2. Skim the page's topic sections to review the main ideas.
3. Use the **Glossary** to check the vocabulary.
4. Drill the **Flashcards** until you can answer every card.
5. Take the **Quiz** to test yourself.

## Project architecture

```
.
├── README.md
├── index.html             home page: links to every chapter
└── study-pages/
    ├── ch01-study.html
    ├── ch02-study.html
    └── ...                one file per chapter: chNN-study.html
```

The site is served by **GitHub Pages** straight from the repository root: `index.html` is the home page, and each chapter lives at `https://sofien6.github.io/Designing-Data-Intensive-Applications-2nd-edition/study-pages/chNN-study.html`.

### One page = one chapter

Every page is a **single self-contained HTML file** with no build step, framework, or backend:

- **HTML:** the content (summaries, glossary, flashcards, quiz).
- **Inline `<style>`:** all styling, including light and dark themes.
- **Inline `<script>`:** all interactivity (flashcards, quiz).
- **External:** only Google Fonts. Without a connection, the page still works and falls back to system fonts.

Because of this you can open a page offline, host it on any static host, or share it as one file.

### Page layout

Each page follows the same structure:

| Section | Purpose |
|---------|---------|
| Header + table of contents | Chapter title and jump links to every section |
| Topic sections | The chapter's main ideas, summarized (one `<section>` per topic) |
| Glossary | Key terms and short definitions |
| Flashcards | Click to flip; use them to drill recall |
| Quiz | Multiple-choice questions with feedback |

### Features

- **Light and dark mode:** follows your operating system's setting automatically.
- **Progress saved locally:** flashcard and quiz progress is stored in your browser's `localStorage`. It stays on your machine, and clearing site data resets it.
- **Responsive:** works on phones as well as desktops.

## Contributing

Corrections and new chapters are welcome.

- Name new pages `chNN-study.html` (zero-padded chapter number) and put them in `study-pages/`.
- Keep the same self-contained structure: inline CSS and JS, no build tools.
- Add a card for the chapter in `index.html` and a row in the table above.
- Open a pull request with a short description of what you changed.

## Disclaimer

This is an unofficial study companion. _Designing Data-Intensive Applications_ is © O'Reilly Media and its authors. The summaries here are written in my own words for learning purposes.
