---
name: crit-prompt
description: Crit a prompt for an AI tool — a generator (Midjourney, Magnific, Runway, Figma Make) or Claude itself (chat, Claude Code, artifacts, project or skill instructions) — to surface the context still in the creative's head. Use when a designer says "crit my prompt", "is this prompt good", or shares a prompt before generating or sending it to Claude.
---

Read [`../crit-shared/METHOD.md`](../crit-shared/METHOD.md) and run it on the user's **prompt**. Whatever reads the prompt can't see into the user's head: a generator can't ask follow-up questions, and Claude fills most gaps with a plausible guess. Every gap becomes a guess — your job is to find the gaps first.

## The tree

Confirm which tool the prompt is for (alongside the discipline check), then take that tool's branch. Ask each root branch only where the prompt is missing it, and tailor the questions and the rewrite to what that tool responds to.

### Generators (image, video, UI)

Tailor to parameters and aspect ratio flags for image models, camera movement and duration for video models, layout and interaction for UI generators.

- **Subject**: what, exactly, is in frame?
- **Style**: medium, era, references, artist or studio influences.
- **Mood and light**.
- **Composition**: framing, angle, aspect ratio.
- **Motion** (video): what moves, how, and for how long.
- **Exclusions**: what must not appear.
- **Purpose**: where the output goes, which sets resolution and format.

### Claude

Claude reads a prompt like a capable collaborator on their first day: keywords matter less than context and intent. First pin down the surface — a chat, a Claude Code build, an artifact, or standing instructions (a project, skill or system prompt) — since it sets what the output is and what "done" means.

- **Task**: what Claude makes or does, and the deliverable: copy, a brief, ideas, a critique, a prototype, a site.
- **Context**: the project, client, audience and history Claude has no way to know. Which files, links, brand guidelines or Figma frames go in with it?
- **Voice or look**: tone and reading level for words; references, type, colour and layout for anything visual.
- **Constraints**: length, brand rules, tech stack for builds, the deadline if it changes scope — each with its reason, since Claude generalises from the why.
- **Output format**: structure, length, file type, and where the output goes next.
- **Success**: how the user will judge the result. One example of good beats any adjective.
- **Process**: should Claude ask questions first, offer options, plan before building, or just go?

Write the rewrite as plain prose, with a short heading or XML tag around each block of pasted material. Phrase exclusions as the behaviour wanted ("write in short, plain sentences" over "don't be wordy").

### The closing check

"Has this got the most context possible?" is the heart of this mode: push it until nothing in the user's head is missing from the prompt.

## Finishing

Replace the standard recap with:

1. **The rewritten prompt** in a code block, ready to copy, in the target tool's syntax.
2. **What was missing**: a short list of the gaps you filled, so the user learns to include them next time.
3. Any parked branches.

## Running it

Offer to run the prompt. Confirm first and run only on a clear yes.

- **Generators**: when the target tool is connected in this session (Magnific, Figma, Photoshop generative tools, Blender generation — check with ToolSearch), name the tool and any credit cost.
- **Claude**: this session already holds the whole crit, so running the prompt here hides its gaps. Offer a **cold read** instead: dispatch a subagent with only the rewritten prompt and its attachments, then show the user what came back and any gap it exposed. For a prompt that builds or changes files, hand it over to run in a fresh session.

Next command: `/crit-work` once there's output to look at.
