# DESIGN.md

The design guide for surajkohli.com. Every page on the site follows it.

It was built by studying ten personal sites from people in the same space as Suraj: engineering and product leaders, crypto builders and investors, and the design engineers whose sites set the bar for this genre. Screenshots of each (1200×800 viewport, captured 23 Nov 2026) are in the project folder at `surajkohli.com-preview/references/`. The numbers below were read from each site's computed CSS, not estimated from the images.

**The niche, in one line:** a product and engineering leader who builds teams and does serious blockchain work, and who wants to be hired as a consultant. The site has to read as *credible, calm and technical*, not as a portfolio or a startup landing page.

---

## 1. The ten references

| # | Site | Who | Why it's here |
|---|------|-----|---------------|
| 1 | [leerob.com](https://leerob.com) | Product at SpaceX, ex-Vercel | Product/eng leader, serif warmth, best bio pattern |
| 2 | [cdixon.org](https://cdixon.org) | a16z crypto | Crypto thought leader, best editorial list |
| 3 | [samczsun.com](https://samczsun.com) | SEAL founder, ex-Paradigm | Web3 security, technical-but-polished tone |
| 4 | [karrisaarinen.com](https://karrisaarinen.com) | Linear CEO | Founder writing about building teams and quality |
| 5 | [lethain.com](https://lethain.com) | Will Larson, eng exec author | The engineering-leadership reference in this niche |
| 6 | [stephango.com](https://stephango.com) | Obsidian CEO | Warm palette, quiet structure, great dark mode |
| 7 | [paco.me](https://paco.me) | Design engineer, Linear | Three-column project grid, link-as-content |
| 8 | [brianlovin.com](https://brianlovin.com) | Designer at Notion | Two-line identity hero, icon social row |
| 9 | [paulstamatiou.com](https://paulstamatiou.com) | Head of Design, Sesame | Serif + sans pairing, one disciplined accent |
| 10 | [emilkowal.ski](https://emilkowal.ski) | Design engineer, ex-Linear/Vercel | Extreme restraint, spacing as the only decoration |

---

## 2. What makes each one work

### 1. leerob.com
- **Layout:** One 600px text column on the left; the right side of the screen is a single large illustration. The bio is two short paragraphs, then "Notes" as a two-column list of links, then "Blogs" as rows with a right-aligned date. A small **Default / Long** tab lets the reader pick how much bio they want.
- **Type:** Iowan Old Style (a serif) for everything. Body 17px / 1.6. Name 42px, weight 600, tracking −0.02em. Section heads 23px. Dates switch to a 14px system sans in grey, which separates metadata from content without a second color.
- **Color:** Pure white, ink `#282828`, muted `#676767`. Links are grey with a 30%-opacity underline. No accent color at all.
- **Spacing:** ~48px between sections, 1em between paragraphs, rows separated by hairlines.
- **Steal:** the two-paragraph bio, the Default/Long toggle, faint underlines.

### 2. cdixon.org
- **Layout:** A 656px centered column. Header row: name, a one-line italic tagline, and a four-item nav pushed right. The home page *is* the essay list: title on the left, date on the right, a hairline between every row.
- **Type:** Newsreader (serif) for titles at 18px; dates in IBM Plex Mono at 12px with +0.06em tracking, grey. Serif + mono is the whole system.
- **Color:** Warm paper `#F7F5F0`, ink `#1C1A17`, muted `#6F6A61`. Nothing else.
- **Spacing:** Rows are ~35px tall with 1px dividers; ~48px from header to list.
- **Steal:** the paper background, serif titles with mono dates, and the row list. This is the most "crypto-credible" look of the ten: it feels like a publication, not a project.

### 3. samczsun.com
- **Layout:** A 632px centered column. Logo + name on the left of the header, six mono nav links on the right. Then an "ABOUT" section of two paragraphs and a "WRITING" list where each row has a title, a one-line description under it, and a mono date on the right.
- **Type:** System sans body at 16px / 1.6. Section labels in ui-monospace, 13px, weight 600, uppercase, +0.05em, grey. Nav is mono too.
- **Color:** `#FAFAFA` background, ink `#171717`, muted `#666666`. Links stay ink-colored with a grey underline.
- **Spacing:** ~40px between sections; list rows ~52px with dividers.
- **Steal:** the mono uppercase section label (it signals "engineer" without saying it) and the title + description + date row. This is the closest match to a security/protocol consultant.

### 4. karrisaarinen.com
- **Layout:** A narrow 432px column. A tiny avatar + name header, "About me" in three lines, then **"Notes on building"**: a list of one-line principles ("Small teams create better work", "Quality earns trust…").
- **Type:** System sans at 14px / 1.7, weight 400. Section heads are the *same size* as body, set apart only by weight 600. Dates at 11px grey.
- **Color:** White, ink `#292824` (warm near-black), muted `#77746D`.
- **Spacing:** Generous: ~36px between sections, ~20px list rows.
- **Steal:** the principles list. For an engineering leader, a short list of how you build teams says more than a résumé.

### 5. lethain.com
- **Layout:** A wide header (site name left, five nav links right), then a 736px column: a one-paragraph intro with book links, then a dated list of posts.
- **Type:** Avenir Next throughout at 16px / 1.5. Site name at 24px, weight 200 (light), which is the one stylish move.
- **Color:** White, black text, **default browser-blue underlined links** (`#0000EE`).
- **Spacing:** Rows ~34px, no dividers.
- **Steal:** the dense, dated list that proves output over time. **Avoid:** default blue links and unstyled underlines. This site shows that content can carry a leadership brand, but it is the plainest of the ten and the one to learn *least* from visually.

### 6. stephango.com
- **Layout:** A 666px column. Header: name left; About, Now and a theme switch right. Sections are labelled in grey ("Latest", "Topics", "Writing") and separated by full-width hairlines. The writing list uses a fixed-width date column (`2025 · 10`) followed by the title.
- **Type:** System sans at 18px / 1.5. Headline 20px, weight 500, tracking −0.015em. Metadata 16px in grey.
- **Color:** Cream `#FFFCF0`, ink `#100F0F`, muted `#6F6E69` (from his own Flexoki palette, which has a matching dark mode).
- **Spacing:** ~64px between sections with a divider in the middle of each gap.
- **Steal:** the warm cream base, the divider-between-sections rhythm, and the fixed date column.

### 7. paco.me
- **Layout:** A 640px column. Name, a two-sentence intro, then a **three-column grid** (Building / Projects / Writing) where each item is an underlined title with a two-line description underneath, and ↗ marks external links.
- **Type:** Söhne (a grotesk sans) at 16px / 1.75, with one *italic serif* phrase in the intro ("Crafting interfaces") as the only flourish. Column labels at 14px.
- **Color:** White, ink `#3A3A3A` (soft, never pure black), underlines in the same color.
- **Spacing:** ~48px between blocks, ~24px between grid items. The page fades in on load.
- **Steal:** the three-column "what I'm doing" grid without cards, the ↗ external-link mark, and one serif italic accent.

### 8. brianlovin.com
- **Layout:** A 640px column starting about 200px down the page. Name, then the one-line role statement at the same size in grey, then a row of three social icons, then a short "Writing ›" list.
- **Type:** Inter. Name and role are both 24px, weight 600; the name is near-black and the role is grey `≈#555`. Same size, two tones is the whole hero.
- **Color:** White, near-black, mid grey. No accent.
- **Spacing:** Very large top padding, ~40px between hero, icons and list.
- **Steal:** the two-tone hero (identity in ink, what you do in grey, same size) and icon-only social links.

### 9. paulstamatiou.com
- **Layout:** A 576px column offset right of a slim vertical icon rail (Home, About, Talks, Photos, theme). Hero is name + two short paragraphs; then **Posts / Favorites** tabs and a list of title + one-line description.
- **Type:** A custom serif (PSC) for name (29px, 550) and post titles; a humanist sans (PSA) for tabs and descriptions. Body 18px / 1.5.
- **Color:** Warm oatmeal `#F7F2ED`, ink `oklch(0.37 0.01 68)` (a brown-black), muted text at 90% of a taupe. One accent: an olive green used **only** for the active nav icon.
- **Spacing:** Hero starts ~110px down; ~60px between hero and tabs; ~20px between list items.
- **Steal:** a serif headline with sans support text, and the rule that the accent color appears in one place only.

### 10. emilkowal.ski
- **Layout:** A 450px column. Name and title stacked as two lines, then sections ("Today", "Projects", …) separated by ~80px of empty space. No dividers, no images, no cards.
- **Type:** One sans at 14px / 1.65. Labels weight 500, body 400. Nothing larger than 16px on the page.
- **Color:** `#FDFDFC` off-white, ink `#21201C`, muted grey, underlines in a light `#BCBBB5`.
- **Spacing:** This site's only design device. Big gaps between sections, tight gaps within them.
- **Steal:** confidence in whitespace. If a section feels crowded, add space before adding a line or a box.

---

## 3. What the ten have in common

These patterns showed up on at least seven of the ten sites, so treat them as rules.

1. **One narrow column.** Median content width is **~640px**, never wider than ~740px. Left-aligned text inside a centered column.
2. **Name, not a slogan, at the top.** Most open with the person's name and a plain one-line role. None uses a big marketing headline.
3. **Off-white, near-black, one grey.** Six of ten use a warm off-white; ink is never `#000`; the muted grey is warm (`#666`–`#77746D`).
4. **Almost no accent color.** Links are ink or grey with a soft underline. Only one site (paulstamatiou) has a true accent, and it appears in one place.
5. **No cards.** Content sits on the page, separated by space and hairlines, not by boxes, shadows or rounded panels.
6. **Small headings.** Section labels are 13–20px, often the same size as body text, set apart by weight, color or a mono face.
7. **Lists, not grids of tiles.** Work and writing are shown as rows: title, an optional one-line description, metadata on the right.
8. **Metadata gets its own voice.** Dates and tags switch to mono or smaller grey text so they never compete with titles.

---

## 4. The surajkohli.com system

This is what every page uses. It keeps what already works on the current site (Inter, JetBrains Mono, light/dark toggle, the Product / Blockchain / Leadership story) and moves the look toward the references: paper background, no cards, no indigo, a serif voice for headlines.

### 4.1 Layout

- Content column: `max-width: 640px`, centered, left-aligned text.
- Page gutter: `20px` on each side at all widths (`24px` from 768px up is fine).
- Header: name on the left, 3–4 nav links and the theme toggle on the right, `32px` from the top. The header uses the same 640px column as the content.
- The hero starts `96px` below the header on desktop, `56px` on mobile.
- No sidebars, no full-bleed sections, no background panels. One column from top to bottom.
- Multi-column only for short link lists (like paco.me's 3-up grid): `grid-template-columns: repeat(3, 1fr)` at ≥640px, one column below.

### 4.2 Typography

| Role | Font | Size / line-height | Weight | Tracking | Color |
|------|------|--------------------|--------|----------|-------|
| Name / page title | Newsreader (serif) | 34px / 1.15 (28px on mobile) | 500 | −0.015em | `--ink` |
| Hero statement | Inter | 20px / 1.5 | 400 | −0.01em | `--muted` |
| Section label | JetBrains Mono | 12px / 1.5, uppercase | 500 | +0.08em | `--muted` |
| Item title | Inter | 16px / 1.5 | 500 | normal | `--ink` |
| Body | Inter | 16px / 1.7 | 400 | normal | `--ink` |
| Item description | Inter | 15px / 1.6 | 400 | normal | `--muted` |
| Metadata (dates, tags) | JetBrains Mono | 12px / 1.5 | 400 | +0.04em | `--muted` |

- Load: `Newsreader:opsz,wght@6..72,400;6..72,500` (and the italic 400), `Inter:wght@400;500;600`, `JetBrains+Mono:wght@400;500`.
- Exactly three faces, each with one job: serif speaks (name, page titles, essay titles), sans explains, mono labels.
- One serif italic phrase per page is allowed as an accent (paco.me), for example in the hero.
- Never go above 34px. Never use weight 700. Prose measure stays under 68ch.

### 4.3 Color

```css
:root {
  --bg:     #F7F5F0;  /* warm paper (cdixon, stephango) */
  --ink:    #1C1A17;  /* warm near-black, never #000 */
  --muted:  #6F6A61;  /* warm grey for support text and labels */
  --line:   #E4E0D8;  /* hairlines and dividers */
  --hover:  #EFECE5;  /* row hover wash */
  --accent: #2F6F4E;  /* deep green; focus rings, active nav, the one primary button */
}
:root[data-theme="dark"] {
  --bg:     #151412;
  --ink:    #ECE9E2;
  --muted:  #9C968B;
  --line:   #2A2824;
  --hover:  #1D1B18;
  --accent: #7FB89A;
}
```

- Links: `color: var(--ink)`, underline in `--line` (or the ink at 30% opacity), `text-underline-offset: 3px`. On hover the underline turns `--ink`.
- The accent appears in **at most two places** on a page: the active nav item or focus ring, and the single primary action. It never colors body links, headings or borders.
- Green is chosen over the current indigo because indigo/purple is the default "crypto startup" color; a muted green reads as calm and solvent, and none of the references use purple.
- No gradients, no shadows, no glassmorphism, no neon. Dark mode is a warm charcoal, not pure black (stephango, samczsun).

### 4.4 Spacing

A 4px base, using only these steps: `4, 8, 12, 16, 24, 32, 48, 64, 96`.

- Between sections: `64px` (desktop), `48px` (mobile). Optionally a `1px var(--line)` divider halfway, as on stephango.com.
- Section label to its content: `16px`.
- Between paragraphs: `16px`.
- List rows: `14px` vertical padding, `1px var(--line)` divider between rows (cdixon, samczsun). Title to description: `2px`.
- Grid gaps: `24px` column and row.
- If something feels crowded, add space before adding a border.

### 4.5 Components

Every page is built only from these.

- **Header.** Name (serif, 17px, links home), nav links in Inter 14px `--muted` (active link is `--ink`), theme toggle as a bare 16px icon with no border.
- **Hero.** Name/title in the serif, then a 1–2 sentence statement in the 20px muted sans (two-tone, like brianlovin.com), then at most one primary action and one plain text link.
- **Section label.** Mono, uppercase, 12px, muted (samczsun). No `h2` larger than this on the home page.
- **Row list** (work, writing, talks). Title on the left, optional description beneath in muted, metadata in mono on the right, hairline between rows, a `--hover` wash on hover. External links end with `↗`.
- **Three-up link grid** (focus areas). Label, then underlined title, then a two-line description. No boxes.
- **Principles list** (engineering leadership). Short one-line statements, each under ~60 characters, like Karri Saarinen's "Notes on building". Up to eight.
- **Consulting block.** Same column, same background. Set apart by a section label and a top divider, not a colored panel. Arrow bullets in `--muted`, one primary button.
- **Primary button.** `--ink` background, `--bg` text, 8px radius, `10px 16px` padding, 14px Inter 500. Hover switches background to `--accent`. One per page.
- **Social links.** Plain text links or 18px monochrome icons in a row (brianlovin). No pills.
- **Footer.** One line: © year and name on the left, a short muted note on the right. Mono 12px.

### 4.6 Motion

- Hover: color and underline transitions at `150ms ease`.
- Optional page fade-in: `opacity 0→1` over `300ms` (paco.me). Respect `prefers-reduced-motion`.
- Nothing else moves.

---

## 5. Rules for every page

1. Start from the header, the 640px column and the footer. Nothing renders outside the column.
2. Open with a serif title and one muted sentence about what the page is.
3. Use section labels, row lists, link grids and prose. If a new component seems necessary, check whether a row list would do first.
4. Use only the tokens in §4.3 and the spacing steps in §4.4. No new colors or one-off pixel values.
5. The accent appears at most twice per page. There is at most one primary button.
6. No cards, pills, tags-as-badges, shadows or rounded panels.
7. Check both themes and a 375px-wide screen before shipping. Body text never drops below 15px on mobile.
8. Keep it plain HTML and CSS with no build step, as the README describes.

---

## 6. What changes from the current site

| Now | Per this guide |
|-----|----------------|
| `max-width: 720px` | `640px` |
| H1 48px bold marketing statement | Serif name 34px/500, statement in 20px muted sans |
| Indigo accent on links, buttons and arrows | Ink links with soft underlines; deep green accent in two places max |
| Bordered rounded cards for "What I do" | Three-up link grid, no boxes |
| Tag pills ("Live · World app") | Mono metadata on the right of each row |
| Highlight panel for Consulting | Same background, section label + divider |
| Pill-shaped social links | Plain text links or monochrome icons |
| `#FAFAF9` cool stone background | `#F7F5F0` warm paper |

The redesign itself is a separate step and has not been started.
