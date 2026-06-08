# Vibe Rise x Indie Campers Pitch Deck Style Guide

## Colors

| Token | Hex | Usage |
|-------|-----|-------|
| Background | `#0a0a0a` | Page background |
| Surface | `#141414` | Cards, boxes |
| Border | `#222222` | Card borders, dividers |
| Text | `#f0f0f0` | Headlines, bold text |
| Text Muted | `#888888` | Body copy, descriptions |
| Accent | `#c850f0` | Labels, handles, highlights |
| Accent 2 | `#ff6b9d` | Gradient end |
| Gradient | `#c850f0 > #ff6b9d` (135deg) | Key headlines, big numbers |
| Growth | `#4ade80` | Positive metrics (+621%, +400%) |

## Typography

**Font**: Inter (Google Fonts), fallback to system sans-serif.

| Element | Size | Weight | Color |
|---------|------|--------|-------|
| H1 (hero title) | clamp(2.5rem, 6vw, 4.5rem) | 900 | White, gradient on "Vibe Rise" |
| H2 (section titles) | clamp(1.8rem, 4vw, 3rem) | 800 | White |
| H3 (card titles) | clamp(1.2rem, 2.5vw, 1.5rem) | 600 | White |
| Body / list items | clamp(1rem, 1.8vw, 1.15rem) | 400 | Muted (#888) |
| Labels | 0.75rem | 700, uppercase, 0.15em tracking | Accent (#c850f0) |
| Handles (@_huzz) | 0.85-0.9rem | 400 | Accent (#c850f0) |
| Big metrics | clamp(2.5rem, 5vw, 3.5rem) | 900 | Gradient |

**Letter spacing**: H1 at -0.03em, H2 at -0.02em. Tight, modern.

## Layout

- Max content width: 900px, centered
- Each section is full viewport height (min-height: 100vh)
- Section padding: 80px vertical, 24px horizontal
- Card border-radius: 16px
- Smaller elements border-radius: 12px
- Card padding: 32px
- Grid gap: 24px

## Components

### Cards (duo-card, metric-card, team-card)
- Background: surface (#141414)
- Border: 1px solid border (#222)
- Border-radius: 16px
- Padding: 32px
- Text: center-aligned

### Video containers
- Border-radius: 16px
- Border: 1px solid border (#222)
- Overflow: hidden
- Videos: autoplay, muted, loop, playsinline
- Hero video: 9:16 aspect ratio, max-width 500px
- Montage video: full width, natural aspect ratio
- Vibe We Create video: 9:16, max-height 75vh, max-width 420px

### Metric rows
- Flex row, space-between
- Top border: 1px solid border (#222)
- Padding: 10px vertical
- Label: muted, Value: white bold

### Route items
- Numbered circles: 28x28px, accent border, accent text
- City name: 1.1rem, weight 600, white
- Landmark: 0.9rem, muted

### Buttons/badges
- Hero badge: pill shape (border-radius: 100px), surface bg, border, muted text
- Pulsing dot: 8px circle, accent color, 2s infinite pulse animation

## Animation

- Fade-up on scroll: elements start at opacity 0, translateY(30px)
- Transition: 0.6s ease on opacity and transform
- Triggered at 15% intersection threshold
- Pulse animation on hero badge dot: opacity 1 > 0.4 > 1, 2s loop

## Tone of Voice

- Short, punchy sentences. No filler.
- Numbers are bold and large. Let the data speak.
- No em dashes. Use periods or commas.
- Section labels are uppercase, small, accent-colored.
- Headlines are statements, not questions.
- Body copy is muted, not competing with headlines.

## Section Hierarchy

1. **Hero** - Title, hook copy, promo video (9:16)
2. **Who We Are** - Montage video, duo cards with bios
3. **Metrics** - Per-account cards, combined bar
4. **The Why** - Thesis statement, brand alignment line
5. **The Vibe We Create** - Event stats headline, event video
6. **The Tour** - Route list with numbered cities
7. **The Content** - Deliverable numbers grid, production team cards
8. **The Partnership** - Value props with icons
9. **The Ask** - Centered box, simple ask
10. **Contact** - Email, handles, links, Jade reference

## Responsive Breakpoints

- Below 640px: duo-grid, metrics-grid collapse to single column. Team grid collapses to single column. Ask box padding reduces.
- All type uses clamp() for fluid scaling between mobile and desktop.

## File Naming

- Videos: lowercase, hyphenated (vibe-rise-hero.mp4, nic-spiff-montage.mp4)
- Images: lowercase, hyphenated (nic.jpg, metrics-nic.png)
- All assets in /public directory
