---
name: GH Plumbing
description: Plumbing fixed, and explained. A calm band site for a plumber who explains before he fixes.
colors:
  copper: "#e0965a"
  copper-bright: "#eaa872"
  copper-ink: "#8a4a1c"
  pipe-blue: "#1b4a7a"
  deep-blue: "#0e2238"
  paper: "#f4f6fb"
  light-band: "#e7ecf4"
  card-white: "#ffffff"
  field-tint: "#e6ecf5"
  ink: "#0e2238"
  body-slate: "#2a3a4c"
  soft-slate: "#4a5868"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  hairline: "rgba(14,34,56,.12)"
  error-red: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  phone-display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 9vw, 52px)"
    fontWeight: 400
    lineHeight: 1
  card-title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(24px, 6.4vw, 30px)"
    fontWeight: 400
    lineHeight: 1.1
  title-desktop:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "22px"
    fontWeight: 400
    lineHeight: 1.2
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "21px"
    fontWeight: 400
    lineHeight: 1.2
  title-small:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  promise:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.7vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: ".02em"
rounded:
  focus: "6px"
  field: "10px"
  row: "20px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  card-pad: "22px"
  stack: "16px"
  band: "64px"
  band-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.copper}"
    textColor: "{colors.ink}"
    typography: "{typography.title-small}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.copper-bright}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.title-small}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-ghost-hover:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.on-dark}"
  input-field:
    backgroundColor: "{colors.field-tint}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field-tint}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card-white}"
  card-tip:
    backgroundColor: "{colors.card-white}"
    textColor: "{colors.body-slate}"
    rounded: "{rounded.card}"
    padding: "22px 22px 26px"
  card-form:
    backgroundColor: "{colors.card-white}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  eyebrow-pill:
    backgroundColor: "rgba(14,34,56,.06)"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
  step-number:
    backgroundColor: "{colors.copper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.copper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
  facebook-row:
    backgroundColor: "{colors.deep-blue}"
    textColor: "{colors.on-dark}"
    rounded: "20px"
    padding: "14px 16px 14px 22px"
    height: "72px"
---

# Design System: GH Plumbing

## Overview

**Creative North Star: "The Basement Explainer"**

The plumber who explains, rendered as Ellie's calm band style: copper pipe and brass valves in an unfinished basement, seen under a navy wash, then a page of full-bleed bands that alternate off-white paper with pipe-blue and deep blue. Nothing shouts. Each band holds one idea, set in a single rounded display face (Cal Sans) over a plain system body, and the only warm colour on the page is copper, used the way the trade uses it: as solid material, never as thin lettering on light ground.

Density is low and phone-first. Everything is one column at 390px with a 20px gutter; desktop widens the gutter, splits a few bands into two columns, and otherwise just breathes (96px band padding). Shapes are soft and borderless: 24px cards, full pills, tinted 10px fields. Depth comes from band contrast and photo overlays, not from shadows; the floating call circle is the single lifted object.

Motion is limited to three gestures: the hero H1 bounces in letter by letter once, content below the first screen rises 12px into place once, and the floating circle slides up after the hero leaves. All three disappear under reduced motion, and nothing is ever left hidden without JS.

**Key Characteristics:**
- Paper, two blues, one copper accent; copper is a fill, `copper-ink` is its text form on light.
- Full-bleed bands in a fixed light/dark rhythm under the photo hero: paper, deep (textured), the paper form band (only when texting is on), light, navy, then the deep footer.
- One display webfont (Cal Sans, weight 400 only) for headings, buttons, labels and phone numbers; system stack for body at 16/1.7.
- Soft borderless geometry: 24px cards, 999px pills, 10px tinted fields.
- Flat surfaces; one shadow in the whole system (the floating circle).
- Calling is the primary action; texting features exist but are gated behind `CONFIG.TEXTS`.
- Every photo is an AI-generated example of a problem, never presented as the client's work.

## Colors

A cool, papery blue-grey world with a single warm metal accent.

### Primary
- **Copper Pipe** (copper): the one accent, used only as a fill: primary buttons, the numbered step discs, the floating circle, the eyebrow dot, text selection. Text on it is always Ink. Inside dark bands and the hero it may also colour text (the accent phrase in a headline, the phone glyph on the closing number), because it clears contrast on deep blue.
- **Bright Copper** (copper-bright): hover state of copper fills only.
- **Copper Ink** (copper-ink): copper as text or line-icon on light grounds (about 6:1 on paper): the accent phrase in a light-band headline, the "What we fix" icons, the header phone glyph and its hover, tip-card run-in labels.

### Secondary
- **Pipe Blue** (pipe-blue): the mid navy. The closing "Need plumbing help?" band, and the colour of every focus outline and form hover border on light grounds (kept distinct from the copper fill so focus never looks like a button).
- **Basement Deep** (deep-blue): the dark band ("How it works"), the footer, the hero's base and overlay tint, the Facebook row, the brand tile, and the fallback behind photos. On bands and the footer it always carries the line texture.

### Neutral
- **Paper** (paper): page ground, header, and light content bands. Never replaced with white or black as a page ground.
- **Light Band** (light-band): the alternate light band (homeowner tips), one step cooler than paper so the band edge reads.
- **Card White** (card-white): tip cards and the form card, sitting on paper or light band.
- **Field Tint** (field-tint): inputs and chips on white cards. It exists because paper on white is about 1.08:1 and fails non-text contrast.
- **Ink** (ink): headings and labels on light, text on copper, the selected chip fill. Same value as Basement Deep, kept as its own role.
- **Body Slate** (body-slate): running text on light.
- **Soft Slate** (soft-slate): ledes, placeholders, helper text, the "(optional)" marks.
- **On-Dark** (on-dark) and **On-Dark Soft** (on-dark-soft): headings and body text on navy, deep and the hero. Hero H1 and photo-card titles go to pure white.
- **Hairline** (hairline): the only divider: between "What we fix" rows and above tip-card advice.
- **Error Red** (error-red): inline error sentences and the error border on a field.

### Named Rules
**The Copper Is Metal Rule.** Copper is a fill, never thin text on a light ground. On paper, light band or white, any copper-coloured text or line icon uses Copper Ink; on deep blue, navy or the hero, true copper is allowed.

**The Blue Focus Rule.** Focus and form hover on light grounds are Pipe Blue outlines (3px, 3px offset); on navy, deep, the hero and the footer they switch to copper. Focus is never signalled by a copper fill.

**The Textured Deep Rule.** Every deep-blue band and the footer carry `repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`. Never stronger than about 4% white, so it can't read as lines through text. Pipe-blue bands stay plain.

## Typography

**Display Font:** Cal Sans (with "Avenir Next", "Segoe UI", system-ui, sans-serif)
**Body Font:** System stack (-apple-system, BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif)

**Character:** Cal Sans is round, friendly and a little chunky, which suits a tradesman who talks plainly; the system body keeps long explanations fast and native in Facebook's in-app browser. Cal Sans ships one weight and is always set at 400; hierarchy comes from size alone.

### Hierarchy
- **Display** (400, clamp(42px, 12vw, 80px), 1.02): the hero H1 only, max 11ch, white, last phrase in copper. The only heading that animates.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): section H2s. Balanced wrapping.
- **Phone Display** (400, clamp(30px, 9vw, 52px), 1): the closing tap-to-call number, with a phone glyph at 0.8em.
- **Title** (400, 21px, 1.2; 22px on wide screens): step titles and the wordmark; tip photo titles run larger (clamp(24px, 6.4vw, 30px), 1.1) and "What we fix" rows at clamp(20px, 5.4vw, 24px), 1.15.
- **Title Small** (400, 18-19px, 1.2): buttons (18px, line-height 1), form labels, tip-card terms, header phone number.
- **Lede** (400, clamp(17px, 4.6vw, 19px)): one sentence under a section heading, Soft Slate, max 38ch. The hero promise is its sibling at clamp(17px, 4.7vw, 20px), 1.5, max 30ch on phones.
- **Body** (400, 16px, 1.7): all running text. Inputs are 16px so iOS never zooms.
- **Label** (500, 14px, .02em): the eyebrow pill text and the "(optional)" helper.

### Named Rules
**The One Display Face Rule.** Cal Sans carries every heading, button, form label, list title and phone number; the system stack carries everything you read in sentences. No third family, no second display weight.

**The Number Is Display Rule.** Phone numbers are always set in Cal Sans, never wrap (`white-space: nowrap`), and appear in three places only: header top-right, the closing band, and the footer.

## Layout

A single centred column (max 1160px) with a 20px gutter on phones, 40px from 760px. Bands are full-bleed with 64px vertical padding on phones and 96px from 760px; the band itself is the section divider, so there are no rules between sections.

Section heads stack eyebrow, headline and lede with 16px gaps, left-aligned, max 640px wide. From 760px the hero copy gains height (120px top / 136px bottom), the hero buttons sit side by side at a 240px minimum, and the tip cards become two equal columns. From 1024px "What we fix" splits head and list into two columns (64px gap), the three steps run in a row (40px gap), the closing band puts headline left and the big number right, and the form section pins its head sticky beside the card.

Band order as built: paper header, photo hero, paper ("What we fix"), deep ("How it works"), paper form (hidden unless texting is on), light ("Homeowner tips"), navy (close), deep footer. Light and dark alternate so every new section is obvious.

Tap targets are 44px or larger everywhere (header links, footer links, buttons at 56px, chips at 48px, the float at 60px). The footer reserves 96px plus the safe-area inset at the bottom so the floating circle never covers it.

## Elevation & Depth

The system is flat. Depth is conveyed by band contrast (paper against deep blue), by white cards sitting on tinted grounds, and by photo overlays: the hero photo under a navy gradient (0.86 to 0.6 vertically on phones; 0.90 to 0.45 left-to-right on desktop) and each tip photo under a bottom gradient to 0.92 deep blue so its white title reads.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(8,24,46,.3)`): the floating call circle only, because it sits over every band.

### Named Rules
**The One Shadow Rule.** Only the floating circle casts a shadow. Cards, buttons, pills and the header are flat at rest and on hover.

## Shapes

Soft and borderless. Cards round to 24px, the Facebook row to 20px, fields and the brand tile to 10px, and every button, chip and eyebrow is a full pill (999px). Step numbers, the arrow disc and the float are true circles. Borders appear only as state (a 2px transparent border that becomes Pipe Blue on hover/focus or Error Red on error) or as the 1px hairline divider. Photos are clipped by their card's radius and always `object-fit: cover`, never stretched; tip photos are 4:5 on phones and 4:3 from 760px.

## Components

### Buttons
Big, soft and unmistakable.
- **Shape:** full pill (999px), 56px tall, 26px side padding, Cal Sans 18px.
- **Primary:** Copper fill, Ink text, copper 2px border. Hover (pointer devices only) goes to Bright Copper.
- **Ghost:** transparent with a 2px border at 70% on-dark, on-dark text; used only on the hero beside the primary. Hover whitens the border and adds a 10% white wash.
- **Press:** scales to 0.98 over 120ms. Colour transitions run 200ms.
- **In the form:** full width; hover and focus add a 2px Pipe Blue outline at 2px offset.
- At most two buttons in the hero: one filled, one ghost. There is no Call button in the hero; the number lives top-right.

### Chips
- **Style:** Field Tint pill, 48px tall, 18px padding (14px under 380px), system 16px Ink text, 2px transparent border.
- **State:** hover border Pipe Blue; selected fills Ink with white text; keyboard focus is a 3px Pipe Blue outline at 3px offset (a border alone is invisible on the ink fill).

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** Card White on paper or Light Band.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none; internal advice blocks are separated by a hairline.
- **Internal Padding:** 22px sides, 26px bottom on tip cards; clamp(20px, 5vw, 32px) on the form card.

### Inputs / Fields
- **Style:** Field Tint fill, no visible border at rest (2px transparent), 10px radius, 52px minimum height (textarea 120px), 16px system text, Pipe Blue caret.
- **Focus:** border turns Pipe Blue (no glow). Hover does the same on pointer devices.
- **Error:** border Error Red, kept even while focused, plus a plain-sentence error line below in Error Red.
- **Labels:** Cal Sans 18px Ink, `for`-linked; "(optional)" in 14px Soft Slate.

### Navigation
- **Header:** paper strip, 64px (76px from 760px), wordmark left (a 34px deep-blue rounded tile with copper "GH", hidden under 375px, then "GH Plumbing" in Cal Sans 21/24px), tap-to-call number right with a Copper Ink phone glyph. Hover turns the number Copper Ink.
- **Footer:** textured deep blue, name and number, a Facebook link in on-dark; links are 44px tall and turn copper on hover.

### Eyebrow Pill
A quiet label above a few key headings (the hero, the tip band, the form): 14px/500 system text, a 7px copper dot, a 6% ink wash on light or 12% white on dark, pill radius. Never a button: no arrow, no hover, no shadow, no full copper fill, and never marked up as a heading. This is Ellie's documented house-style exception to the Impeccable rule against eyebrows; it is capped at those few headings and is not to spread to every section.

### Homeowner Tip Card
The client's own Facebook tip posts, rebuilt. A white 24px card: a 4:5 (4:3 on desktop) generated example photo with a bottom deep-blue gradient and the question as a white Cal Sans title on it, then a definition list of causes (Cal Sans 19px terms, body definitions), then "What you can do" / "Homeowner tip" advice behind a hairline, with the run-in label in 14px uppercase Cal Sans, .06em, Copper Ink. The uppercase label belongs to this card only, because it mirrors the wording on the client's own posts.

### Facebook Row
A deep-blue textured 20px-radius row, 72px tall, Facebook glyph and "See more of our tips on Facebook" in Cal Sans, with a 44px arrow disc at 12% white. On hover only the arrow disc changes, filling copper with Ink arrow; keyboard focus puts a copper outline on the disc. Half the content width on desktop.

### How It Works Steps
A numbered list on the textured deep band: 48px copper discs with Ink Cal Sans numerals (CSS counter), on-dark Cal Sans titles, on-dark-soft body. One column on phones, three across from 1024px.

### Floating Call Circle
One 60px copper circle, bottom right inside the safe area, with an Ink phone glyph and the float-lift shadow. It slides up (350ms, cubic-bezier(.2,.8,.2,1)) once the hero has scrolled away and slides away while the control it duplicates is on screen: the closing phone number by default, the text form when texting is on. While hidden it gets `tabIndex=-1` and `aria-hidden`. `CONFIG.FLOAT = false` removes it. It is a circle, never a bottom bar.

### Texting Gate (CONFIG.TEXTS)
Calling is primary because the owner hasn't confirmed the number takes texts. `CONFIG.TEXTS = false` (shipped) keeps the "Tell us what's wrong" form band hidden, points the hero primary button at the closing call band, and makes the float a `tel:` link. Setting it `true` reveals the form band, retargets the hero button to it, and turns the float into an `sms:` link with a pre-written greeting and a chat glyph. The form composes a text from name, problem, town and "how soon" chips, and falls back to a "Didn't open your messages? Call us" line after 900ms.

### Motion
- **Hero H1 bounce-in:** JS splits the hero H1 into letters inside nowrap word spans (keeping the accent span); each letter goes from opacity 0 and 50px right to rest over 1s on `cubic-bezier(.34,1.56,.64,1)`, 20ms apart. The H1 carries an `aria-label` during the run, letters are `aria-hidden`, and the plain HTML is restored on the last `animationend`. Skipped entirely without JS or under reduced motion.
- **Rise:** elements marked rise fade up 12px over 400ms ease-out on entering the viewport, and only if they started below the first screen. Visible at rest, without JS, and under reduced motion.

## Do's and Don'ts

### Do:
- **Do** use copper only as a fill (buttons, step discs, the float, the eyebrow dot), with Ink text on it; switch to Copper Ink for any copper text or icon on paper, light band or white.
- **Do** alternate full-bleed light and dark bands, and give every deep-blue band and the footer the 135° line texture at about 3.5% white.
- **Do** set every heading, button, label and phone number in Cal Sans 400, and running text in the system stack at 16px / 1.7.
- **Do** keep shapes soft and borderless: 24px cards, 999px pills, 10px Field Tint inputs.
- **Do** keep tap targets at 44px or more and fields at 16px text.
- **Do** keep calling primary and leave the text form and texting float behind `CONFIG.TEXTS` until the owner confirms texts.
- **Do** label every generated photo as an example: each shipping raster gets an `img/*.json` sidecar with a "GENERATED: model, date, example of ... (not a GH Plumbing job)" prompt line, and alt text describes the problem, not a job.
- **Do** confine hover styles to `(hover: hover)` and drop all motion under `prefers-reduced-motion`.

### Don't:
- **Don't** set copper (#e0965a) as text on a light ground, or white text on a copper fill.
- **Don't** add shadows to cards, buttons, pills or the header; the floating circle is the only lifted object.
- **Don't** animate any heading other than the hero H1, and don't leave any content at opacity 0 without JS or under reduced motion.
- **Don't** add a bottom call bar, a second floating control, or a Call button in the hero.
- **Don't** put an eyebrow pill above every heading, give it a hover, arrow or shadow, or mark it up as a heading.
- **Don't** present a generated image as GH Plumbing's work, its crew, or its van; generated photos illustrate problems only.
- **Don't** stretch photos; use `object-fit: cover` and re-crop instead.
