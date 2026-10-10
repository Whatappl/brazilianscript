<div align="center">

<img src="https://cdn.phototourl.com/member/2026-10-10-37264725-7f3b-4b0d-aade-93a68df460df.png" alt="Fearless FFH4X" width="180" />

# Fearless FFH4X

**Free Fire scripts, configs and tools — delivered clean.**

[![Website](https://img.shields.io/badge/site-brazilianscript.netlify.app-00c853?style=for-the-badge)](https://brazilianscript.netlify.app)
[![YouTube](https://img.shields.io/badge/YouTube-@fearlessxitt-red?style=for-the-badge&logo=youtube)](https://www.youtube.com/@fearlessxitt)

</div>

---

## What this is

The public hub for Fearless FFH4X — a small, focused collection of tools and drops for Free Fire players. One landing page, live counters, a gate that unlocks the download, and a multilingual interface.

Everything is client-side. No trackers. No ad networks. No data leaves your browser.

**Live:** [brazilianscript.netlify.app](https://brazilianscript.netlify.app)

---

## Features

**Landing page**
- Multilingual UI — English, Español, Português, Indonesia, العربية
- Automatic RTL flip for Arabic
- Live visit counter, downloads counter, live viewer estimate
- Countdown to next drop
- Join gate — download unlocks after the four channels are opened
- Live poll — global votes, real numbers
- Device detection — Android / iOS strip
- QR code for desktop users
- Progressive Web App prompt
- Lite mode for slow connections
- Confetti on unlock
- Auto-refresh chip — "updated Xs ago"

**Fearless AI** *(/ai.html)*
- Streaming replies, word by word
- Stop mid-generation
- Regenerate any reply
- Copy any reply
- Conversation memory in `localStorage`
- Voice input
- Model picker, tone, length, language lock
- Suggestions panel — type any category, get 20 fresh feature ideas

**Fearless Toolbox** *(/toolbox.html)*
- Password generator — `crypto.getRandomValues()`, length + charset controls
- Hash tool — SHA-256 / SHA-1 / SHA-512 for text and files
- Encode / decode — Base64, Hex, URL, ROT13
- Password strength — real entropy, crack-time estimate, live check pills

---

## Stack

| Layer | What |
|---|---|
| Hosting | Netlify (static, free tier) |
| Frontend | Plain HTML + CSS + JavaScript — no framework, no build step |
| Fonts | Sora + JetBrains Mono + Noto Kufi Arabic via Google Fonts |
| Counters | [abacus.jasoncameron.dev](https://abacus.jasoncameron.dev) — free, no signup |
| AI | Google Gemini via a Netlify Function (key never touches the browser) |
| QR | `api.qrserver.com` |

**One HTML file per page. No `node_modules`. No bundler. Opens in any browser.**

---

## Project structure
