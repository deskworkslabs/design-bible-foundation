---
name: design-bible-foundation
description: Use before judging, critiquing, or improving any visual design — a UI, a page, a poster, a deck — when the goal is to tell whether it looks "polished," "cheap," "cramped," or "upscale," and to name exactly why, in checkable terms rather than vague taste.
license: MIT
---

# AI Design Bible — Foundation

AI assistants are routinely asked to make something "look more polished"
or "less cheap" or "more premium," and just as routinely produce
confident, vague answers — more padding here, a nicer font there — without
a shared, checkable vocabulary for what those words actually mean. This
skill is that vocabulary: concrete, visually-checkable criteria for the
handful of qualities people mean by "good design" but rarely define.

This is the free Foundation tier of a larger Design Bible. It covers the
baseline vocabulary everyone needs. The paid Professional tier expands
each section below into its own deep-dive with a reference asset pack;
Enterprise adds a live MCP connector version of the whole thing. None of
that is required to get value from this file on its own.

## The five qualities, defined concretely

Each of these is a word people throw around freely. Each has a concrete,
checkable test below it — not "does it feel premium" (unanswerable) but
"does it pass this specific check" (answerable by looking).

### 1. "Polished" vs. "rough"

Polish is **consistency under scrutiny** — the same decision applied the
same way everywhere, with no exceptions nobody can explain.

Checkable tests:
- Do all corner radii in the design come from the same small set of
  values (e.g. 4px / 8px / 16px), or is every element radius whatever
  felt right in the moment? Mixed arbitrary radii (6px here, 11px there)
  read as unpolished even when each one individually looks fine.
- Do icons share a stroke weight, a corner style, and a visual size,
  or is each icon from a different source/style? A mixed icon set is
  one of the fastest ways to make an otherwise-good design look rough.
- Is spacing built from a scale (e.g. 4/8/12/16/24/32/48/64px) applied
  consistently, or are gaps eyeballed per-element? Polish shows up as
  the absence of "almost-aligned" — elements that are nearly but not
  quite on the same grid line read as more careless than elements that
  are visibly, intentionally off-grid.
- Do interactive elements (buttons, links, inputs) have one consistent
  hover/focus/active treatment across the whole surface, or does each
  screen invent its own?

### 2. "Cheap-looking" vs. "premium-feeling"

Cheap is not about color saturation or how expensive the content is —
it is almost always about **unresolved tension**: things fighting for
attention with nothing actually prioritized, or decoration applied
without a reason.

Checkable tests:
- Count how many different accent colors, font weights, or shadow
  styles compete on one screen. Cheap-looking designs usually have too
  many things trying to be the most important element at once; premium
  designs have a clear, obvious single focal point per view.
- Look for decoration with no functional reason: a gradient on a button
  that serves no purpose, a shadow under flat elements with no implied
  light source, a border around something that doesn't need separating
  from its neighbor. Premium design uses visual weight (color, shadow,
  size, contrast) only where it's doing a job — directing attention,
  showing state, implying hierarchy.
- Check whitespace at the edges and between major sections. Cramped
  margins and tight section gaps are one of the single strongest cheap
  signals — premium design is *generous* with space around what matters,
  because space itself communicates confidence that the content doesn't
  need to be crammed in to justify its presence.
- Look at how text wraps and breaks. Orphaned single words on their own
  line, ugly mid-word breaks, ALL CAPS used for anything longer than a
  short label — these are small details that compound into "cheap" even
  when the big-picture layout is fine.

### 3. "Cramped" vs. "breathing room"

This is almost entirely about **the ratio of content to space around
it**, and specifically about *consistency* of that ratio.

Checkable tests:
- Measure the gap between a block of text and the edge of its
  container. Is it the same gap used elsewhere for a similar
  relationship, or smaller just because "it needed to fit"? Cramped
  design usually isn't uniformly tight — it's *inconsistently* tight,
  with some elements getting generous space and others squeezed because
  the designer ran out of room and shrank margins instead of rethinking
  content.
- Check line-height on body text. Anything under roughly 1.4–1.5x the
  font size on paragraph text reads as cramped regardless of how much
  margin surrounds the block — line-height inside a text block matters
  as much as the margin around it.
- Look at information density per view. Cramped isn't "too much
  content" in the abstract — it's too much content with no grouping.
  The fix for cramped is almost never "make it smaller," it's "group it
  so the eye processes it in chunks instead of one undifferentiated
  mass."

### 4. "Upscale" vs. "budget"

Upscale is best understood as **restraint plus precision** — fewer
elements, each one more deliberately placed and more carefully finished,
rather than more elements or more expensive-looking materials.

Checkable tests:
- Count distinct font sizes used across a design. Budget designs tend
  to have many slightly-different sizes (16px here, 17px there, 15px
  somewhere else); upscale designs use a small, deliberate type scale
  (e.g. 4–6 sizes total) applied consistently.
- Check alignment discipline: do elements align to a consistent grid
  (left edges lining up, consistent column widths), or does each
  section use its own ad-hoc layout? Rigorous alignment, more than any
  single visual choice, is what separates upscale from budget — it's
  invisible when done right and glaringly obvious when absent.
- Look at image and photo quality/cropping. Budget designs often use
  stretched, low-res, or awkwardly-cropped images; upscale designs
  either use genuinely good imagery or deliberately avoid photography
  where good imagery isn't available, rather than using mediocre
  photography to fill space.
- Check color restraint: how many distinct hues appear? Upscale
  palettes are typically built from one or two core hues plus neutrals,
  with color used sparingly and purposefully; budget designs often use
  many saturated hues competing for attention.

### 5. "Modern" vs. "dated"

This one ages faster than the others and is the hardest to give
permanent rules for, but a few durable signals exist:

Checkable tests:
- Shadows: heavy, dark, hard-edged drop shadows (especially with visible
  offset and no blur) read as dated; soft, subtle, low-opacity shadows
  with larger blur radii read as current. This has been broadly true
  across design eras, even as exact shadow values trend.
- Gradients: harsh, high-contrast gradients across just 2 very different
  hues read as dated (especially diagonal ones used decoratively);
  subtle, low-contrast gradients within a single hue family (used for
  depth, not decoration) read as current.
- Borders: thick, high-contrast borders on every container read as
  dated; current design tends to separate sections with spacing and
  subtle background shifts rather than hard borders everywhere.
- Corner radii: very sharp (0px) or very round (pill-shaped/fully
  rounded everything) both carry era signals depending on context —
  check what's currently in active use in the specific product category
  being designed for, rather than assuming one radius style is
  universally current.

## How to use this when reviewing a design

1. Don't start with "I don't like it" or "make it more premium" — name
   which of the five qualities is actually failing (usually it's 2–3 of
   them at once, not one).
2. For each failing quality, run its checkable tests above and point to
   the *specific* element that fails the test, not a vague area of the
   screen.
3. Fix the specific, named issue, not "the overall feel." Fixing three
   named, specific problems (inconsistent corner radii, a fighting
   color palette, cramped section margins) produces a visibly better
   result than one vague pass at "making it nicer."
4. Re-run the same checks after the fix — polish and upscale in
   particular are about *consistency*, so a fix applied to one element
   but not its siblings can make things look more inconsistent, not
   less.

## What this skill does not do

- It does not replace a trained designer's eye for novel, genuinely
  creative direction — it gives a shared vocabulary and checkable floor,
  not a ceiling on what's possible.
- It is not a brand-identity or illustration-style guide — it covers the
  structural/systemic qualities of a design (consistency, spacing,
  restraint, alignment), not taste in color or imagery style, which is
  legitimately subjective and brand-specific.
- It does not cover accessibility contrast ratios, motion design
  principles, or component-level UX patterns in depth — those are
  covered in the Professional tier's expanded, per-domain files.
