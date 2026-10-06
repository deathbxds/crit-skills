---
name: crit-prompt
description: Crit a prompt for an AI tool (Midjourney, Magnific, Runway, Figma Make, Claude, etc.) to surface the context still in the creative's head. Use when a designer says "crit my prompt", "is this prompt good", or shares a prompt before generating.
---

Read [`../crit-shared/METHOD.md`](../crit-shared/METHOD.md) and run it on the user's **prompt**. The tool can't ask follow-up questions, so every gap becomes a guess — your job is to find the gaps first.

## The tree

1. **Target tool**: confirm which tool the prompt is for (alongside the discipline check). Tailor the questions and rewrite to what that tool responds to: parameters and aspect ratio flags for image models, camera movement and duration for video models, layout and interaction for UI generators, role and output format for LLMs.
2. Root branches, each asked only where the prompt is missing it:
   - **Subject**: what, exactly, is in frame?
   - **Style**: medium, era, references, artist or studio influences.
   - **Mood and light**.
   - **Composition**: framing, angle, aspect ratio.
   - **Motion** (video): what moves, how, and for how long.
   - **Exclusions**: what must not appear.
   - **Purpose**: where the output goes, which sets resolution and format.

The closing check — "Has this got the most context possible?" — is the heart of this mode: push it until nothing in the user's head is missing from the prompt.

## Finishing

Replace the standard recap with:

1. **The rewritten prompt** in a code block, ready to copy, in the target tool's syntax.
2. **What was missing**: a short list of the gaps you filled, so the user learns to include them next time.
3. Any parked branches.

## Running it

If the target tool is connected in this session (Magnific, Figma, Photoshop generative tools, Blender generation — check with ToolSearch), offer to run the prompt. Confirm first, naming the tool and any credit cost, and run only on a clear yes.

Next command: `/crit-work` once there's output to look at.
