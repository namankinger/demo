---
name: preserve-references
description: Turn Pinterest boards, saved images, links and animation clips the user supplies into a structured reference board and design brief for Preserve (tin, T-shirt, unboxing, lid card, reels, motion). Use when the user says "references", "moodboard", "inspiration", "Pinterest board", "animation references", "motion references", "find similar designs", or shares images or links as design inspiration. Does not scrape Pinterest.
---

# Preserve References

Builds a reference board and design brief from material the user provides. It does not search or scrape Pinterest, because Pinterest restricts automated scraping and results are often blocked.

## Before you start

1. Read `.agents/brand-context.md` (brand, audience, tone). If it is missing, run the `brand-context` skill first.
2. Read `.agents/references/` if it exists, so new material adds to the board instead of replacing it.

## Accepted inputs (ask the user to provide at least one)

- Images or screenshots saved from Pinterest, Instagram, Behance or anywhere else.
- A Pinterest board or pin URL. Fetch only the page the user pointed to; if it cannot be read, ask for exported images instead.
- Links to animation, motion or reel examples, with a note on what they like about each.
- A short description of what to find ("hand-painted tins", "slow reveal unboxing").

## Process

1. **Sort every reference into one bucket:**
   - Object: tin, painting style, lid card, label, typography
   - Apparel: T-shirt print, fit, fabric feel, colour
   - Unboxing: layering, reveal order, packaging materials
   - Plant: marigold, growing kit, bloom moments
   - Reel and motion: hooks, pacing, hands-at-the-bench shots, transitions
   - Page and social: layout, typography, feed look
2. **For each reference record:** source (URL or file name), bucket, what to learn from it (one sentence), and what to avoid copying.
3. **Extract patterns, not pictures:** colour families, type styles, materials, camera angles, pacing, transitions. Name 3 to 5 patterns per bucket.
4. **Motion references:** for animation, note timing and easing in plain terms (slow start, snap, settle), the length of the first 3 seconds, and what the viewer sees first. Use the animation skills in `.claude/skills/` (for example `timing-calibration`, `attention-management`) for deeper timing advice.
5. **Check against the brand:** drop or flag anything that conflicts with the brand context (for example loud urgency styling when the tone is calm).
6. **Write the brief** to `.agents/references/reference-board.md` using the template below.

## Rules

- Treat references as inspiration. Never reproduce another maker's work, logo or artwork, and say so in the brief.
- Credit the source for every reference. If the source is unknown, write "source unknown".
- Do not invent references, URLs or artists. If nothing was provided, ask for material.
- Do not state facts about the product that are UNKNOWN in the brand context (fabric, sizes, tin size, Archive 002 details). Mark design ideas as proposals.

## Output template

```markdown
# Preserve Reference Board

## Summary
[2 to 3 sentences on the overall direction]

## Object
- Reference: [source] | What to learn: [..] | Avoid copying: [..]
- Patterns: [3 to 5]

## Apparel
...

## Unboxing
...

## Plant
...

## Reel and motion
- Reference: [source] | Hook: [..] | Pacing: [..] | Easing: [..]
- Patterns: [..]

## Page and social
...

## Conflicts with the brand
[anything flagged]

## Next step
[one concrete test, for example: shoot two 3-second reel openings from the same paint session]
```
