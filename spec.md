# Tech — tech.christophergoulet.com

## Role

The Tech page demonstrates depth and shows off the cool stuff. It serves two audiences simultaneously:

1. **People evaluating Christopher for hire** (CTOs, technical founders, engineering leads) — needs to demonstrate competency, depth, and a point of view quickly
2. **Peers and open source users** — wants to see what's been built (Phonon, The House), understand the philosophy, and maybe contribute or use

**The feeling after 5 minutes:** "This person genuinely understands distributed systems. They have a coherent philosophy about infrastructure. And they've actually shipped real things."

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
[Nav — brand + "Book a call" CTA]
[Hero — terminal boot sequence, title, subtitle, actions]
[Section 01 — Philosophy / point of view]
[Section 02 — What I build (service cards)]
[Section 03 — Current builds (Phonon, The House)]
[Section 04 — Archive (selected work log)]
[Booking panel]
[Footer]
```

### Hero

- Boot sequence (same animated pattern — "initializing the house", "discovering nodes via mDNS", "pairing · ed25519", "routing · health-aware", "all nodes nominal")
- Title: "Resilient infrastructure. Sovereign systems."
- Subtitle / lede: "I build systems that don't phone home. Distributed inference clusters, private AI stacks, zero-trust networks, and agent systems — all designed for one-person operation." 
  - OR, from Christopher's interview: "I speak human and computer fluently. I see connections others cannot. And I center people while doing it."
  - Suggested: Use Christopher's words as a pull quote or tagline under the main lede. "I speak human and computer fluently" is too good to bury.
- Actions: "Start a conversation" (copper btn-primary) + "See what I've built" (btn-ghost, linking to #builds)

**No stats panel in the hero.** The boot sequence + terminal aesthetic + copper/teal palette is enough visual identity. A stats panel here would compete with the solarpunk feel.

### Philosophy Section

This section exists because tech pages that only list services feel like a menu. Christopher's philosophy about systems is a differentiator.

**Section header:** "A point of view" / "Systems that last are systems that can evolve"

**Content (drawn from interview):**
- "You don't design a program to last forever. You design a system to surface problems, address those problems, collaborate with stakeholders, and work on a continuous feedback loop."
- "Systems that last are systems that can evolve, flex, be better over time."
- The isomorphism: cookies and software are both source code → pipeline → package → deploy. "I generate isomorphic systems for values-based endeavors."

This section can be a pull quote, a short paragraph, or the proof block (with copper border instead of amber-dim). Keep it tight — 3-4 sentences. It's the "why" before the "what."

### Services Section

6 service cards in 3-column grid. Same .serve card pattern but with copper underline on hover.

**Section header:** "What I build" / "Full-stack systems engineering for people who need it to last"

1. **Infrastructure & DevOps** — Design, deployment, and hardening. TrueNAS, Traefik, Authentik, Docker Compose, Tailscale, Nebula. Stacks one person can operate.
2. **Private AI Infrastructure** — On-premise LLM inference, Phonon cluster, model distribution. No cloud, no data leakage.
3. **Security & Resilience** — Architecture-level review, threat modeling, hardening. I find what automated scanners miss — logic errors, design assumptions, dead code paths.
4. **Agent Systems** — Multi-agent architectures, autonomous operations, self-maintaining infrastructure. The House is the proof case.
5. **Cooperative Technology** — Platform co-op design, member-owned systems, democratic governance. Technology that gives people ownership.
6. **Audio & Electronics** — Studio design, signal flow, live venue sound. The technical side of the craft, from someone who's toured New England.

### Current Builds Section

Two build cards (same pattern as current tech page).

**Section header:** "Current builds" / "What I'm building now"

1. **Phonon** (IN DEVELOPMENT) — "A private distributed inference cluster. Turn spare Android phones into a secure, private AI cluster. No cloud, no data leakage. mDNS discovery, Ed25519 pairing, health-aware routing. Open source."
2. **The House** (SELF-HOSTED) — "A multi-agent system for generational sovereignty. A self-maintaining infrastructure stack whose agents observe, document, and improve the systems they run on. Built so one person can operate at the scale of many."

These should link to the respective repos or project sites when they exist.

### Archive Section

Log-format archive (same pattern as current). Tech-relevant only.

**Active:** Uproot Technology LLC (2013–), Phonon (2026–), The House (2025–), Covered Bridge Cooperative (tech infrastructure work)
**Completed:** Keyscrape (2014 — SSH key distribution research), Wotown (2015 — location-based mobile app), Hanover Stringed Instruments GM (2009–2017)

## What NOT to include

- No Covered Bridge story here (that's biz's proof block)
- No Selectboard experience (that's civic)
- No diaspora content (that's canada)
- No pain questions (the biz framing)
- No bilingual toggle
- No carnival feel (civic)
- No stats panel in hero

## OLED

Near-black (`#0a0b0d`) is fine here — the tech page has more visual chrome (terminal boot, mesh canvas, service cards) so true black isn't as critical. But don't use light backgrounds anywhere.

## Tech Notes

- Single-file HTML. Inline CSS. Inline SVG defs.
- Mesh canvas is appropriate here — copper node connections with teal "healthy" nodes. The existing canvas JS can be adapted with new colors.
- Boot sequence animation fits perfectly. Keep it.
- Scroll reveal on sections is fine.
- The copper/teal palette needs to be tested on dark background — copper especially can disappear if it's too dark. It needs to glow, not blend.

## Open Questions

1. **Copper color** — what exact hex? `#c87a3f` is a starting guess. Need to test on dark background for contrast.
2. **Teal color** — `#3fa8a8` is a starting guess. Should teal be the link/button color and copper the heading/mono accent? Or vice versa?
3. **The isomorphism framing** — "cookies and software are both source code → pipeline → package → deploy." This is Christopher's best metaphor. Should it be its own section, or worked into the philosophy section?
