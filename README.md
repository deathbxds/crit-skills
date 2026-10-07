# crit-skills

Claude Code skills that run a creative-director crit on graphic, motion and visual art work.

| Skill | Use it for |
|---|---|
| `/crit-concept` | Turning a raw idea into a clear vision |
| `/crit-brief` | Stress-testing a project brief: scope, audience, deliverables, constraints |
| `/crit-prompt` | Tightening a prompt for an image, video or UI generator (Midjourney, Runway, Figma Make…) or for Claude itself |
| `/crit-work` | Feedback on a work in progress: a screenshot, Figma link or open Photoshop file |

Suggested flow: `crit-concept → crit-brief → crit-prompt → crit-work`.

All four share the method in `crit-shared/METHOD.md`, so keep that folder next to them.

## Install

Copy the five folders into your personal skills folder:

```bash
git clone https://github.com/deathbxds/crit-skills.git
cp -R crit-skills/crit-* ~/.claude/skills/
```

Then start a new Claude Code session.
