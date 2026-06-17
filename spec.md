# Tech — tech.christophergoulet.com

## Role

The Tech page is a show-and-tell for a geek who builds cool things. It's not selling anything — the contact buttons exist but they're not the point. This is where Christopher gets to be the builder, the tinkerer, the person who turns spare Android phones into inference clusters because that's a fun problem to solve.

**The feeling after 5 minutes:** "This person builds really interesting things. I want to see what they make next."

## Aesthetic Direction

**Solarpunk retro-futurism, executed through the visual language of the early web.** This is the key design constraint for the tech page.

**What this means:**
- The copper/teal solarpunk palette stays — the sincerity and optimism are what make this work
- But the visual execution channels Geocities, Angelfire, the web of 1996–2003
- Page counter at the bottom of the page. Not a joke — a real page counter rendered in classic style (e.g., the "digit" counter GIFs or a CSS version of the same)
- A web ring. Links to the other four subdomains in classic web-ring format: "← christophergoulet.com → biz → tech → canada → civic" with a small graphic. This replaces the standard footer link list
- Marquees? Maybe one, used sparingly, for something that genuinely benefits from motion (e.g., the terminal boot output)
- Solid background colors in table cells or panel headers (Geocities-era layout principle)
- Star or sparkle dividers between sections instead of thin horizontal rules
- Under construction GIF icon. Not ironic — sincere. "This site is always under construction" is the exact right philosophy for a solarpunk builder
- A guestbook or "sign my guestbook" link (could be a Cal.com booking redirect framed as a guestbook)
- The "made with" footer badge: "Made with ☕ and 🍪 in Windsor, VT" or similar
- Construction / terminal aesthetic: semi-transparent scanlines, monospace-heavy, but with the copper warmth bleeding through

**Key principle:** This is NOT parody. It is not ironic 90s nostalgia. It is an earnest expression of the web's original vision — personal, handmade, expressive, non-commercial — filtered through a modern solarpunk lens. The sincerity is what makes it work. If it feels like a joke, it's wrong.

**What this is NOT:**
- Not skeuomorphic (no beveled buttons trying to look like Windows 95)
- Not ironic (no Comic Sans, no "you've got mail" popups)
- Not retro-bait (no Matrix green-on-black hacker aesthetic)
- Not corporate tech (no clean blue Salesforces)
- Not straight-laced minimal (no heydonworks restraint here)

**Color palette (draft — iterate):**
- Background: `#0a0b0d` (existing dark is fine — the warmth comes from the accents, not the background)
- Primary accent: Copper — `#c87a3f` (warm, metallic, amber-but-different)
- Secondary accent: Teal — `#3fa8a8` (organic, living, technical)
- Text: warm white `#e6e8ea`
- Muted text: `#9aa1a9`
- Terminal green: keep `#6cc49a` or shift to a warmer green (`#8cb87a`)
- Scanline: existing pattern, warm the opacity slightly

## Content Architecture

```
[Nav — brand]
[Hero — terminal boot sequence, title, lede, actions]
[Section 01 — Current projects]
[Section 02 — Areas]
[Guestbook panel]
[Footer]
```

### Hero

- Boot sequence (same animated pattern — "./house up", "mDNS service discovery", "ed25519 pairing", "health-aware routing", "all nodes nominal")
- Title: "Systems online."
- Lede: "Private AI, distributed inference, agent systems. human/computer fluency."
- Prompt: "$ whoami"
- Bio blurb: 3-5 sentences describing who Christopher is — Franco-Canadian builder, cookie maker who builds systems, worker-owned bakery + multi-agent stack, municipal service, cooperative conversions, distributed systems. "I build things that last and don't phone home."
- Actions: "Message me" (gold btn-primary, mailto link) + "GitHub" (btn-ghost, links to github.com/chezgoulet)

No stats panel, no pitch copy. The boot sequence + title + lede + bio blurb is the whole statement.

### Current Builds Section

Two build cards (same pattern as current tech page).

1. **Phonon** (IN DEVELOPMENT) — "A private distributed inference cluster. Turn spare Android phones into a secure, private AI cluster. No cloud, no data leakage. mDNS discovery, Ed25519 pairing, health-aware routing. Open source."
2. **The House** (SELF-HOSTED) — "A multi-agent system for generational sovereignty. A self-maintaining infrastructure stack whose agents observe, document, and improve the systems they run on. Built so one person can operate at the scale of many."

These should link to the respective repos or project sites when they exist.

### Areas Section

Six technical areas, listed like files in a directory — short, lowercase, no numbering. Each has a `>` prompt prefix and a one-line description.

- **infra/devops** — TrueNAS, Traefik, Tailscale, Docker Compose, Nebula. Stacks one person can operate.
- **private AI** — On-prem LLMs, distributed inference clusters. Your data stays on your hardware.
- **security** — Architecture review, threat modeling. What automated scanners miss: logic errors, design assumptions, dead code paths.
- **agent systems** — Multi-agent orchestration, autonomous operations. Systems that observe and improve themselves.
- **cooperative tech** — Member-owned platforms, democratic governance. Infrastructure that matches how your organization runs.
- **audio/electronics** — Studio design, live sound, signal flow. From clubs to recording studios — I know my way around a board.

### Archive Section

Log-format archive (same pattern as current). Tech-relevant only.

**Active:** Uproot Technology LLC (2013–), Phonon (2026–), The House (2025–), Covered Bridge Cooperative (tech infrastructure work)
**Completed:** Keyscrape (2014 — SSH key distribution research), Wotown (2015 — location-based mobile app), Hanover Stringed Instruments GM (2009–2017)

## What NOT to include

- No Covered Bridge story (that's biz)
- No Selectboard experience (that's civic)
- No diaspora content (that's canada)
- No pain questions (the biz framing)
- No bilingual toggle
- No carnival feel (civic)
- No pitch copy in the hero
- No "I can help you" framing

## OLED

Near-black (`#0a0b0d`) is fine here — the tech page has more visual chrome (terminal boot, mesh canvas, area list) so true black isn't as critical.

## Tech Notes

- Single-file HTML. Inline CSS. Inline SVG defs.
- Mesh canvas is appropriate here — copper node connections with teal "healthy" nodes. The existing canvas JS can be adapted with new colors.
- Boot sequence animation fits perfectly. Keep it.
- Scroll reveal on sections is fine.
- The copper/teal palette needs to be tested on dark background — copper especially can disappear if it's too dark. It needs to glow, not blend.

## Open Questions

1. **Copper color** — what exact hex? `#c87a3f` is a starting guess. Need to test on dark background for contrast.
2. **Teal color** — `#3fa8a8` is a starting guess. Should teal be the link/button color and copper the heading/mono accent? Or vice versa?
