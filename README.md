# Plainsight

A dictionary for people who were never given one.

114 cybersecurity terms, each explained in four sentences and an analogy. Eleven of them don't just explain — they demonstrate, live, on your own browser, or animate step by step.

**[Open it →](#)** *(add your live link here)*

---

## Why

Security is taught in words you don't have yet, about machinery you can't see. Certificates, cookies, handshakes, keys — all of it happens in a fraction of a second, invisibly, and then you're expected to discuss it.

Most explanations fix this by using more words. This one shows you the thing.

---

## What it does

**An index of 114 terms**, in seven sections: Watching you, Locks and keys, Ways in, Ways to stop it, Under the hood, The job and its words, and AI security.

Every entry has the same five parts, always in the same order:
- a one-sentence summary
- **In plain words** — three or four sentences, no unexplained jargon
- **Think of it like** — the analogy
- **Why it matters** — the common misunderstanding, where there is one
- a live demo or diagram, on the eleven that have one

**Eight entries run on your own browser.** Cookie sets and deletes a real one. Browser fingerprint lists what the page learned about you the moment it loaded, including a canvas fingerprint. Hashing and Salt compute SHA-256 as you type. Encoding does base64 both ways to prove no key was ever involved. Entropy measures a password, then explains honestly why the number it just showed you is probably optimistic.

**Three entries animate the machinery.** The TLS handshake, the third-party tracking web, and a man-in-the-middle attack being stopped by a certificate check. Each steps forward one stage at a time with a caption.

**Decode mode.** Paste in a lecture slide, a job posting, an advisory — anything you couldn't read. Every term the book knows lights up. Tap one to jump to its entry.

**An intro screen** that reads five real details off your machine before you go in, to make the point before the first word is defined.

---

## Built with

- **One HTML file.** No framework, no build step, no bundler, no dependencies.
- **Vanilla JavaScript, CSS and inline SVG.** The diagrams are hand-written SVG stepped through with a few lines of script.
- **Web Crypto API** for the live SHA-256 hashing.
- **Google Fonts** — JetBrains Mono, Newsreader, Archivo.

The typography carries the idea: anything in machine-speak is set in the monospace face, anything in human-speak in the serif. You can tell which voice you're reading by the shape of the letters.

---

## Privacy

Nothing leaves your browser. There is no server, no analytics, no network request except the fonts.

The live demos read values your browser hands to every website anyway, and they display them to you and nobody else. The cookie and storage demos write to your own browser and let you delete what they wrote. Your reading progress is kept in `localStorage`, on your machine only.

---

## Running it

Open `index.html` in a browser. That's the whole setup.

To deploy on GitHub Pages: push to `main`, then **Settings → Pages**, source `main` branch, `/ (root)`.

```bash
git clone https://github.com/YOUR-USERNAME/plainsight.git
cd plainsight
open index.html
```

---

## On accuracy

This is a teaching tool, not a specification.

Every definition is simplified on purpose, because a precise definition you can't read teaches nothing. Where simplifying would mislead, the entry says so instead — the entropy demo refuses to call a password strong just because it scored well, the fingerprint demo doesn't claim to uniquely identify you, and the tracking diagram labels its example companies as invented.

Nothing in here was generated at runtime, so nothing can hallucinate. It's a fixed set of written entries plus real values read from your own browser.

If an entry is wrong, open an issue. Especially the cryptography.

---

## What's next

- More terms, in the directions that keep coming up
- More animated machinery — DNS, key exchange, SQL injection
- A quiz mode built from the entries you've already read

---

## Notes

Built as a learning project, by someone studying this and getting tired of being handed vocabulary with no pictures.

The line at the bottom of the page is the whole point:

> Nothing in here was ever hard. It was written by people who already knew, for people who already knew. That is a writing problem, not a you problem.
