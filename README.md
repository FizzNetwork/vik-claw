# vik-claw

Landing page for **Big Vik Claw** — desktop AI assistant by [FizzNetwork.xyz](https://fizznetwork.xyz) / 1UP Media Group.

Live at: **https://claw.viktim.xyz**

## What this repo is

A single-page static site hosted on Vercel. Three files do the work:

| file | purpose |
|---|---|
| `index.html` | landing page — hero, features, integrations, MCP install snippet |
| `oauth-callback.html` | HTTPS hop for OAuth providers that reject `http://localhost` redirects (e.g. Slack). Relays the callback to the local BVC app at `http://127.0.0.1:8477/oauth/callback/<provider>` |
| `vercel.json` | cleanUrls + headers (HSTS, X-Frame-Options, Referrer-Policy, X-Content-Type-Options, Permissions-Policy) |

## Deploy

Connected to Vercel project `vik-claw` via GitHub auto-deploy on push to `main`.
Domain `claw.viktim.xyz` is a CNAME at GoDaddy pointing to Vercel.

Manual preview deploy:

```bash
# from this folder
vercel deploy
```

## Source of truth

This repo is the *deployed* landing. Master copy of the source files lives under the BVC build tree:

```
BigVik-Build/landing/
├── index.html
├── oauth-callback.html
├── vercel.json
├── README.md           <- you are here
├── MICROSOFT-STORE-LISTING.md
└── .gitignore
```

## Where else to find Big Vik Claw

- **Desktop app repo:** github.com/FizzNetwork/bigvik-claw (private)
- **MCP npm package:** `@fizznetwork/vik-mcp-server` — `npx -y @fizznetwork/vik-mcp-server`
- **Support / Telegram:** @viksniperbot
