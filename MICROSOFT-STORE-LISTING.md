# Microsoft Store Listing — Big Vik Claw (Beta)

**Purpose:** Copy-paste ready content for submitting Big Vik Claw to the Microsoft Store.
Fees: one-time $19 individual dev registration. After that, no per-app fee for MSIX packages.

---

## Product Name
Big Vik Claw (Beta)

## Publisher Display Name
FizzNetwork.xyz

## Short Description (150 chars)
Dual-persona desktop AI. Vik builds, Viki posts. Your API keys. 15+ platforms. Works with Claude Desktop, ChatGPT, Cursor via MCP.

## Description (10,000 char limit — under 2,000 is ideal)

Big Vik Claw is a desktop AI assistant with two sides. Vik (he) is your dev partner — reads code, calls MCP servers, manages files, connects to Google / GitHub / Slack / Notion / Figma / Spotify. Viki (she) is your social-posting engine — researches crypto, generates content, schedules across Twitter/X, Telegram, Discord, Bluesky, Mastodon, Reddit, LinkedIn, TikTok, YouTube Shorts, Threads, Farcaster, and more.

**Your keys, your models, your machine.**
- Bring your own API keys — Claude, OpenAI, DeepSeek, xAI. No markup, no proxy, no middleman.
- Or run fully local with Ollama.
- All credentials live in your AppData folder. Never round-trip through our servers.

**OAuth connectors in one click.**
- Google (Gmail, Sheets, Calendar, Drive), GitHub, Slack, Notion, Figma, Spotify.
- Click Connect → browser approve → done. Tokens refresh silently.

**Model Context Protocol (MCP).**
- Use Vik's tools from Claude Desktop, ChatGPT, Cursor, Zed — any MCP-compatible AI.
- Or point Vik at community MCP servers for filesystem, search, databases, and more.

**Social posting at scale.**
- 15+ platforms built in.
- Schedule up to 90 days out.
- Brand card profiles for voice consistency.
- Runs even when the app is closed (Windows Task Scheduler integration).

**What's NOT in the app:**
- Ads. Anywhere. Ever.
- Telemetry you didn't opt into.
- Subscription lock-in — 7-day trial, then an unlock code.

Big Vik Claw is developed by FizzNetwork.xyz / 1UP Media Group.

## Keywords (up to 7)
AI, assistant, desktop, developer, automation, social-media, productivity

## Category
Productivity

## Subcategory
Personal finance / Collaboration  *(closest fit — change if a better one is listed)*

## Age Rating
PEGI 12 / ESRB E10+  *(users can connect apps that contain user-generated content)*

## System Requirements
- **OS:** Windows 10 version 1809+ or Windows 11
- **Architecture:** x64
- **Memory:** 4 GB RAM minimum, 8 GB recommended
- **Storage:** 500 MB
- **Network:** Internet required for AI model API calls and OAuth authentication

## Features (bullets — each 60 char max)
- Two AI personas: Vik for building, Viki for posting
- Bring your own API keys — no markup or proxy
- 15+ social platforms with scheduling
- OAuth connectors: Google, GitHub, Slack, Notion, Figma, Spotify
- MCP server — use Vik from Claude Desktop / Cursor / Zed
- Runs local models via Ollama
- Windows Task Scheduler for offline posting

## Privacy Policy URL
https://claw.viktim.xyz/privacy  *(needs to be live before submission)*

## Support Contact
officialfizznet@gmail.com

## Website URL
https://claw.viktim.xyz

## Screenshots Required (16:10, min 1280x720, max 10)
1. Chat surface with Vik (face + chat bubbles)
2. Viki composing a scheduled post
3. Connections panel with OAuth providers section
4. MCP servers panel (Claude Desktop / community servers)
5. Brand cards editor
6. Multi-platform post preview

## Trailer (optional — strongly recommended)
30-60 second screen capture:
- 0-5s: open app, both faces pulse
- 5-15s: Vik calls a tool (Gmail list), result streams in
- 15-25s: switch to Viki, generate a post, send to scheduler
- 25-30s: Connections panel scroll, tagline card

## Submission Notes for Microsoft
- Requires signing with an EV code-signing certificate (we already have one per package.json build config).
- Electron-builder produces an NSIS installer. To list on MS Store, we'll need to also produce an MSIX package. Add `"target": ["nsis", "msi", "appx"]` to `package.json > build.win` and re-build. MSIX submission may also require a Microsoft Partner Center manual review.
- If MSIX path takes too long, the "app install from the web" card (Desktop App via Windows Package Manager) is a faster entry point — submit to `winget-pkgs` repo as a Manifest PR.

## Timeline
- Get $19 dev account on Microsoft Partner Center (~30 min inc. ID verification).
- Build MSIX package (~1 hour).
- Submit for certification (~3-7 days Microsoft review).
- Fix any cert issues, resubmit.
- Live.

Faster alt: **winget manifest PR**. Takes a couple days, appears in `winget install fizznetwork.bigvikclaw`, zero store fee.
