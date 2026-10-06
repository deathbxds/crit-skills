---
name: crit-work
description: Crit a creative work in progress — a design, frame, sketch, or animation. Use when a designer says "crit this", "give me a crit", or shares a draft, screenshot, Figma link, or open Photoshop file for feedback.
---

Read [`../crit-shared/METHOD.md`](../crit-shared/METHOD.md) and run it on the user's **work in progress**.

## Seeing the work

Look at the work yourself before the first round:

- **Pasted images or screenshots**: view them directly.
- **Figma links**: use the Figma tools (`get_screenshot`, `get_design_context`).
- **Open Photoshop files**: use `photoshop_get_preview` and `photoshop_get_layers`.
- **Motion**: ask for keyframes, a frame strip, or a description of timing and easing.

The crit is read-only: question the work, leave the file untouched. Fixes belong in a separate request the user makes afterward.

## The tree

Root branches:

- **Intent**: what is this meant to do, and for whom? Ask before judging.
- **First read**: what you see first, second, third — and whether that matches the intent.
- **Discipline craft**: the bank for this discipline in METHOD.md.
- **What's working**: name it, so it survives the next iteration.
- **Versions**: 2–3 directions the next iteration could take.

Frame each observation as a question with a recommendation ("The headline and image compete for first read — which should win? ➡️ the image; drop the headline a weight"), so the designer's judgement makes the call.

Done when every observation has a decision or is parked. Next command: `/crit-prompt` if the next iteration will use AI tools, or `/crit-work` again on the revision.
