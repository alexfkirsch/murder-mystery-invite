# Murder Mystery Weekend Invitation Site

## What This Is
A single-page invitation site for a private murder mystery weekend (October 17-19, 2026). Guests receive anonymous physical letters with a unique code word. They visit this site, enter their code word, and see their character assignment, backstory, and event details.

## Stack
- Single index.html file (HTML/CSS/JS, no frameworks)
- Google Fonts only external dependency
- Hosted on Cloudflare Pages (murder-mystery-invite.pages.dev)

## Aesthetic
Old English country manor: dark wood paneling, deep burgundy and mahogany, flickering candlelight effects, wax seal SVG imagery, velvet drape textures, heavy serif typography (Cinzel, EB Garamond). Should feel like opening a sealed letter in a dimly lit study.

## How It Works
1. Splash page: "You Have Been Summoned" with password prompt
2. Each guest has a unique code word that reveals their character
3. Character page shows: name, title, backstory, event details, RSVP buttons
4. RSVP sends email via Formspree (endpoint: https://formspree.io/f/xbdagkzg)
5. localStorage prevents duplicate RSVPs per code word

## Event Details (shown on character page)
- When: October 17-19, 2026
- Arrival: Friday, 5:00 PM
- Where: To be disclosed upon RSVP
- Attire: Period dress mandatory — 1920s country estate
- Secrecy: "Do not speak of this invitation to anyone. Do not attempt to identify the other guests. Do not investigate the address you will be given. Arrive alone."

## Rules
- NEVER attempt to deploy or offer deployment options. Owner deploys manually.
- Always keep everything in a single index.html
- Never run deploy commands
- Preserve the aesthetic on all changes
- Do not modify CLAUDE.md unless explicitly asked

## Deploy (for owner reference only — do not run)
wrangler pages deploy . --project-name murder-mystery-invite --commit-dirty=true
