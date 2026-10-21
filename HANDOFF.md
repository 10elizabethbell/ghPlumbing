# GH Plumbing — handoff at ~60%

**Live:** https://10elizabethbell.github.io/ghPlumbing/ · **Repo:** https://github.com/10elizabethbell/ghPlumbing · **Built:** 2026-10-21 from Muse brief of 2026-10-21 (found via the NJ Home Improvement Contractors Facebook group)
**Call Sheet:** site URL set (entry added; Muse hadn't made one).

## What's built
- One page, calm band style copied from DPG: paper header (GH tile + wordmark left, tap-to-call (551) 998-1338 top right), photo hero under navy, What we fix (paper), How it works (deep navy, 3 steps), Homeowner tips (light band, 2 cards), Need plumbing help? close with the big number (navy), footer (name, phone, Facebook).
- Palette: paper #f4f6fb, pipe-blue #1b4a7a, deep #0e2238, **copper #e0965a** as the one fill accent (ink shade #8a4a1c for text on light). Chosen for the trade: no logo or brand colours could be fetched.
- Hero: generated photo of copper pipes and brass valves in a basement (gpt-image-1) under a navy overlay. Eyebrow "Homeowner plumbing", H1 "Plumbing fixed, and explained." (letter bounce-in), one promise line, two buttons: **Tell us what's wrong** (scrolls to the closing phone number) and **Homeowner tips** (outlined).
- Homeowner tips: the client's own two Facebook infographics rebuilt as cards, their wording kept (one OCR slip fixed: "block redirect" → "block or redirect"; headings dropped their all-caps), then a big "See more of our tips on Facebook" row.
- **Calling is primary** because the brief says texting is unconfirmed. `CONFIG.TEXTS = false` in the script. Flip it to `true` once the owner confirms texts and you get: a "Tell us what's wrong" text form (name, problem, optional town, how soon; composes a pre-written SMS, tested), the hero button pointing at the form, and the floating circle switching from call to text.
- Floating circle (60px, bottom right): currently a **call** circle. Hidden on the hero and while the closing number (or the form, when texting is on) is on screen.
- Fade-up on everything below the first screen; reduced motion and no-JS show everything at once (checked).
- Favicon / home-screen icon: "GH" lettering on deep navy (no logo available). og:image 1200x630 (`og.jpg`).

## Assumptions I made
- **Services list is inferred:** Leaks, Clogged drains, Toilets, Faucets and showers. The brief has no itemized services; these are plumbing basics plus the two things their own posts cover. Confirm before handing over.
- **"We" voice:** the brief doesn't say if it's one person or a crew. "We" reads fine either way; switch to "I" if it's a solo plumber.
- **The GH tile in the header and favicon is the site's own lettering, not their logo.**
- **Positioning "the plumber who explains"** comes from their educational tip posts. The promise ("We tell you what's going on in plain words before we touch a thing") and How it works steps ("We find the cause… then show you what we did") are inferred from that tone, not stated by them.
- **No place in the H1**, against the calm style's rule: the brief says not to publish a location (only the 551 area code and NJ group are known). Add the town/area to the H1 once the owner gives it.
- **Colours:** navy + copper chosen for the trade; the infographics' real colours couldn't be sampled.
- **Name:** "GH Plumbing" exactly; not expanded. Flyers say "GH PLUMBING SERVICES" and there may be a "GHS" mark.

## Placeholders and gaps
- **No logo, no infographic images.** Facebook blocked every fetch (profile and both group posts return the login wall; the Graph picture endpoint returns the blank default). `src-assets/` holds only generated images. Get the logo and the two infographics from the owner or a logged-in browser.
- **All three photos are AI-generated examples** (not the client's work), recorded below. Replace with real job photos when the owner has them.
- No email (footer has none, by the rules), no hours, no service area, no reviews, no licence number, no owner name.

| Image | Used as | Source |
|---|---|---|
| img/hero-800.webp, img/hero-1600.webp | hero background | generated with gpt-image-1, 2026-10-21, prompt: copper supply pipes and brass shut-off valves on an unfinished basement wall, warm bare bulb right, left half in shadow |
| img/tip-shower.webp | showerhead tip card | generated with gpt-image-1, 2026-10-21, prompt: chrome showerhead in white subway tile with mineral scale, crooked jets |
| img/tip-toilet.webp | toilet tip card | generated with gpt-image-1, 2026-10-21, prompt: looking straight down into an open toilet tank, fill valve, flapper, supply line, no bowl (the first version, with a bowl that looked detached from its tank, was replaced on review) |

Provenance sidecars: `img/*.webp.json`. Full prompts in `~/.local/share/genimg/log.jsonl`.

## Questions for the owner
1. Does (551) 998-1338 take texts? (Yes → `CONFIG.TEXTS = true`.)
2. Which towns do you cover? (Goes in the H1 and the close.)
3. What jobs do you take? Emergencies? Water heaters? Drain cleaning? Installs?
4. Your logo and colours, and the original tip graphics.
5. Is it just you or a crew? Your first name for the site?
6. An email for the footer? Hours?
7. Any photos of your own jobs, and any customer reviews we can quote?
8. Licence number (NJ licenses master plumbers individually) if you'd like it shown.

## Ideas not built (yours to pick)
- **Runner-up world (opt-in signature motion):** water. A thin copper pipe running along the hero's bottom edge with a slow drip that gathers and falls when the visitor taps it; or a water line that rises behind the section edges as you scroll. Other worlds considered: brass valve handles that turn as you scroll, a pressure gauge needle, tile grout lines.
- A third tip card each time they post a new infographic (the cards are copy-paste).
- "Before you call" mini-checklist (where's your shut-off valve?) in their homeowner-tip voice.
- Text-to-book per service row, once texting is confirmed.
- Hero eyebrow wording: the sweep suggested "Plumbing for homeowners" instead of "Homeowner plumbing"; the finish reviewer said if eyebrows are ever trimmed, cut this one first ("Save this tip" is the client's own words and earns its place).
- With texting off, "Tell us what's wrong" scrolls a long way (~3,000px on phone) to the closing number. Defensible (it's not a Call button and the close echoes it), but if it feels slow, point it at `#how`.
- Impeccable findings kept on purpose (your calm-style choices): eyebrow pills (craft floor bans kickers), the H1 letter bounce (bounce/elastic easing), the diagonal band texture (detector "repeating-stripes-gradient", ignored for index.html in `.impeccable/config.json`), two hero buttons + the floating circle ("one primary action"). The detector's "flat type hierarchy" was a false positive (it doesn't count the clamp() headings); also ignored there.
- Code hygiene, no visible change: the navy rgba(14,34,56,…) repeats ~8 times; could become a `--deep-rgb` token.

## Not verified
- Real-device tap-to-call and SMS handoff on iPhone / Android / Facebook's in-app browser.
- Real Facebook link preview (og image) until the link is first shared.
- How the generated photos read to the owner. The toilet-tank image has a slightly odd U-shaped tank and the supply line runs through the water; fine at card size, but swap it for a real photo when one exists. A plain navy hero is a one-line swap (remove the `<img class="hero-bg">`).
- Checked headlessly (Chromium + WebKit, 360/390/430/1440): no sideways overflow, tap targets ≥44px, bounce-in starts offset and restores the plain H1 by ~2s, reduced motion and no-JS show everything, float hidden on hero / shown mid-page / hidden at the closing number, hero white text ≥8.5:1 and copper H1 accent ≥3.5:1 by pixel sampling, `CONFIG.TEXTS = true` form path composes and URL-encodes the SMS correctly.
