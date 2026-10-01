---
name: pitch-deck-generator
description: Generate or revise Cloud Grind investor pitch deck content (slides, speaker notes, or a full 15-slide draft) using the established outline, key numbers, and investor messaging rules. Use when asked to draft a pitch deck, write or rewrite a specific slide, prep investor talking points, or update deck numbers for Cloud Grind.
---

# Cloud Grind Pitch Deck Generator

Generates investor-facing pitch deck content for Cloud Grind — individual slides, speaker notes, or a full draft — consistent with the established outline and messaging rules. This is a **project skill**: it only loads in Claude Code sessions working inside this repo (or its clone in a committed cloud session). It is not available in Claude Desktop/claude.ai, which has no project-scoped skills.

## Before writing anything

Read these first, in this order:
1. `PITCH_DECK_OUTLINE.md` (repo root) — the canonical 15-slide structure, headlines, key points, and visual notes per slide
2. `pitch-deck/CLAUDE.md` — investor messaging rules and the numbers to use
3. `BRAND_BRIEF.md` (repo root) — positioning and core promise, for tone consistency outside the investor-specific framing

If `pitch-deck/CLAUDE.md` and this file ever disagree on a number or rule, `pitch-deck/CLAUDE.md` wins — it's the source of truth for this folder.

## Audience and tone

Investors (seed/Series A), partners, press. Confident, minimalist, data-driven — let the numbers and the product speak. Never coffee-snobbery language, never flowery description, never vague market sizing.

## Key numbers (use these, don't invent new ones)

- Target audience: 60% creatives ($60K+ household income), 40% busy professionals ($75K+)
- Price point: $20–28/bag one-time, $18–25/bag subscription (15% off)
- Unit economics: direct trade sourcing at 3x commodity prices, fresh-roasted and shipped within 48 hours
- Market angle: premium specialty without gatekeeping
- Full detailed unit economics, growth targets, and traction numbers live in `PITCH_DECK_OUTLINE.md` (Slides 9 and 11) — pull from there rather than re-deriving

## Messaging rules

✅ Focus on: the market gap (gatekeeping in specialty coffee), unit economics, retention model, founder credibility
✅ Lead with: the problem, then our advantage
✅ Always mention: direct trade sourcing (it's the margin story)
✅ Tone: confident — we know this works, numbers plus conviction

❌ Avoid: coffee snobbery language, flowery descriptions, vague market sizing, product benefits instead of investor benefits

## What to produce

**For a full deck draft:** follow the 15-slide structure in `PITCH_DECK_OUTLINE.md` exactly — same slide order, same headline for each slide unless asked to change it. For each slide, write the on-slide copy (one idea per slide, headline + supporting points) and separate speaker notes (what to say, not what to read — the deck should complement the speaking, not duplicate it).

**For a single slide:** confirm which slide number from the outline, pull that slide's key points and visual notes, and write copy that fits the established pacing (per the outline: spend time on Slides 2–4, breeze through 9–10, land on 14).

**For updated numbers:** if given new traction, revenue, or growth figures, update the relevant slide's numbers only — don't rewrite surrounding copy unless asked, and flag which source number you replaced.

## Output format

Markdown. One `###` heading per slide (`### Slide N: <Title>`), then:
- **Slide copy:** the on-slide headline and bullet points
- **Speaker notes:** 2–4 sentences, conversational, what to say live

## Don't

- Don't invent traction, revenue, or market-size numbers not already in `PITCH_DECK_OUTLINE.md` — ask for them if a slide needs a figure that isn't there
- Don't soften the "zero BS" / anti-gatekeeping positioning into generic premium-brand language
- Don't pull copy from `cold-email/CLAUDE.md` or the customer-acquisition voice — that's a different audience and a different override
