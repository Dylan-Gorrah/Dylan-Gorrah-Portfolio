# New theme revamp (what we’re doing)

We’re taking your current `index.html` (the light / warm “premium” theme) and **revamping it to borrow the vibe from `portfolio_dark.html`**.

When I say “borrow the vibe”, I mean:

- Dark, high-contrast background
- Subtle gold / warm accent glow
- Cleaner “techy” atmosphere (particles / noise / scanlines)
- Dark glass panels and buttons that still feel premium

But we’re **not** copying everything 1:1.

## The rules you gave me

- We’re updating **`index.html`** (this becomes the main file).
- We’re bringing in the **cool dark elements** from `portfolio_dark.html`.
- We’re keeping the typography **subtle and consistent**.
  - One main font used throughout.
- The name **“Dylan Gorrah” should NOT be huge** in the new version.

## What I’m changing first (step-by-step)

1. **Theme + colors**
   - Switch CSS variables to a dark palette.
   - Keep one accent color for highlights.

2. **Background vibe**
   - Add the subtle background layers from the dark theme:
     - particle canvas
     - dot grid
     - scanlines
     - grain/noise
     - soft mouse-follow light (desktop)

3. **UI components**
   - Update the orbit rings and icon chips to look good on dark.
   - Update buttons and the overlay panel to use “dark glass”.

4. **Typography cleanup**
   - Remove the “fancy headline font” look.
   - Keep the whole site on a single subtle font.
   - Reduce the main name size so it looks confident, not shouty.

## What we’re NOT changing

- Your core layout (orbit + panels) stays.
- Your project data (`projects` array) stays.
- Your links (CV download, contact links) stay.

## Goal

When someone opens your portfolio, the first impression should be:

“Clean. Premium. Slightly cyber / modern. Confident.”

…but still readable, professional, and not over-designed.
