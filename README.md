# Shaping Skills (OpenClaw Edition)

[OpenClaw](https://github.com/openclaw/openclaw) skills for shaping and breadboarding — the methodology from [Shape Up](https://basecamp.com/shapeup) adapted for working with an LLM.

Forked from [rjs/shaping-skills](https://github.com/rjs/shaping-skills) and adapted for OpenClaw's skill system.

## Skills

- **shaping** — Iterate on both the problem (requirements) and solution (shapes) before committing to implementation. Separates what you need from how you might build it, with fit checks to see what's solved and what isn't.

- **breadboarding** — Map a system into UI affordances, code affordances, and wiring. Shows what users can do and how it works underneath — in one view. Good for slicing into vertical scopes.

- **breadboard-reflection** — Find design smells in a breadboard and fix them. Works on existing breadboards built with the breadboarding skill.

## Install (OpenClaw)

Skills are symlinked into your OpenClaw skills directory:

```bash
# Clone the repo
git clone https://github.com/Morpheis/shaping-skills.git ~/Personal/shaping-skills

# Symlink each skill into OpenClaw's user skills directory
ln -s ~/Personal/shaping-skills/shaping ~/.openclaw/skills/shaping
ln -s ~/Personal/shaping-skills/breadboarding ~/.openclaw/skills/breadboarding
ln -s ~/Personal/shaping-skills/breadboard-reflection ~/.openclaw/skills/breadboard-reflection
```

Each skill directory contains a `SKILL.md` that OpenClaw discovers automatically.

## Changes from Upstream

- Renamed `skill.md` → `SKILL.md` (OpenClaw convention)
- Ripple-check hook internalized as self-discipline guidance in the shaping skill
- Cross-references updated for OpenClaw skill resolution
- README updated for OpenClaw installation

## Original

Case study: [Shaping 0-1 with Claude Code](https://x.com/rjs/status/2020184079350563263) walks through the full process of building a project from scratch using these skills. The source for that project is at [rjs/tick](https://github.com/rjs/tick).
