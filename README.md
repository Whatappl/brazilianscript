<div align="center">

<img src="https://cdn.phototourl.com/member/2026-10-10-37264725-7f3b-4b0d-aade-93a68df460df.png" alt="Fearless FFH4X" width="160" />

# Fearless FFH4X

**Scripts, configs and tools for Free Fire — built clean, built fast.**

[![Live](https://img.shields.io/badge/live-brazilianscript.netlify.app-00c853?style=for-the-badge&logo=netlify&logoColor=white)](https://brazilianscript.netlify.app)
[![YouTube](https://img.shields.io/badge/YouTube-@fearlessxitt-ff0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@fearlessxitt)
[![License](https://img.shields.io/badge/license-personal-4a9eff?style=for-the-badge)](LICENSE)
[![No trackers](https://img.shields.io/badge/trackers-none-00e05e?style=for-the-badge)](#privacy)

**English** · [Español](#español) · [Português](#português) · [العربية](#العربية)

</div>

---

## Overview

A single static site that serves Free Fire players a set of tools, drops, and an assistant — with nothing running behind it except a Netlify Function for AI. No database, no framework, no build step, no analytics. Loads in under a second on a 3G connection. Works on any phone from 2018 onwards.

Every page is a self-contained HTML file. Edit it in a text editor, drop it into Netlify, done.

**Live:** https://brazilianscript.netlify.app

---

## Table of contents

- [Overview](#overview)
- [What's inside](#whats-inside)
- [Screens](#screens)
- [Stack](#stack)
- [Project structure](#project-structure)
- [Deploy your own](#deploy-your-own)
- [Environment variables](#environment-variables)
- [Editing content](#editing-content)
- [Channels](#channels)
- [Privacy](#privacy)
- [Security](#security)
- [Performance](#performance)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

---

## What's inside

### `index.html` — Landing page

The public hub. Everything a visitor needs in one screen.

- **Gate system** — download stays locked until all four channels have been opened. Progress ring fills in real time. Confetti fires on unlock.
- **Live counters** — total visits, today's visits, downloads, live viewers. Real numbers, real API.
- **Countdown** — to the next drop, in the visitor's local time.
- **Live poll** — global votes on what should drop next. Updates every 30 seconds.
- **Five languages** — English, Spanish, Portuguese, Indonesian, Arabic.
- **RTL support** — the entire layout mirrors when Arabic is selected.
- **Share system** — share sheet on mobile, clipboard fallback on desktop, native WhatsApp Status integration.
- **Device detection** — shows Android users a hint about MT Manager, warns iOS users that the script is Android-only.
- **Progressive Web App** — installable on Android home screen. Works offline for cached pages.
- **Lite mode** — one tap kills every animation and heavy effect for slow connections.
- **QR code** — auto-generated for desktop visitors so they can hand off to their phone.

### `ai.html` — Fearless AI

A working chat interface with streaming replies.

- **Streaming responses** — text types out word by word with a live cursor.
- **Stop generation** — interrupt any slow reply mid-stream.
- **Regenerate** — one tap, new answer, same prompt.
- **Copy reply** — every message has a copy button.
- **Persistent history** — the last 50 messages stay in `localStorage`, safe from a refresh.
- **Voice input** — hold the mic, speak, send. Uses the browser's native speech API.
- **Model picker** — OpenAI, Mistral, Llama, Qwen Coder.
- **Tone and length controls** — casual, formal, brief. Short, normal, detailed.
- **Language lock** — force replies in a chosen language regardless of input.
- **Suggestions engine** — type any category, get 20 fresh feature ideas. Live from the model.
- **Offline guard** — if the network drops, the page shows a red error, not a fake answer.

### `toolbox.html` — Fearless Toolbox

Four independent security and dev tools, all client-side.

- **Password generator** — cryptographically random via `crypto.getRandomValues()`. Length 6–64, customisable charset, "no look-alikes" mode.
- **Hash** — SHA-256, SHA-1, SHA-512 for text and files. WebCrypto, nothing uploaded.
- **Encode / decode** — Base64, Hex, URL, ROT13. UTF-8 safe.
- **Strength tester** — real entropy calculation, time-to-crack estimate, seven live check indicators.

---

## Screens

<div align="center">

<img src="screenshots/landing.png" width="220" alt="Landing" />
&nbsp;
<img src="screenshots/ai.png" width="220" alt="Fearless AI" />
&nbsp;
<img src="screenshots/toolbox.png" width="220" alt="Toolbox" />

</div>

*Screenshots go in a `screenshots/` folder at the repo root.*

---

## Stack

| Layer | Choice | Why |
|---|---|---|
| Hosting | **Netlify** — static, free tier | Push to deploy, zero config, HTTPS included |
| Frontend | **Plain HTML + CSS + JS** | No framework, no build, no dependencies to rot |
| Fonts | **Sora**, **JetBrains Mono**, **Noto Kufi Arabic** | Modern, readable, RTL-aware |
| Counters | **abacus.jasoncameron.dev** | Free, no signup, simple REST, no key |
| AI | **Google Gemini** via Netlify Function | Key stays server-side, generous free tier |
| QR | **api.qrserver.com** | Direct image URL, no library |

**The whole project is three HTML files and one Netlify Function.**

---

## Project structure
