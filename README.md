# unslop (Cursor skill)

Cursor port of [unslop](https://github.com/heydamir/unslop) by Damir Sokolovsky ([@heydamir](https://x.com/heydamir)). Turns vibecoded, AI-looking UI into a designed interface with its own character.

![A vibecoded dashboard unslopping itself, frame by frame](unslop/references/refs/story-dashboard-frames.webp)

## Install

**All projects (recommended)**

```bash
git clone https://github.com/NoahWhiteson/unslop-cursor.git
mkdir -p ~/.cursor/skills
cp -r unslop-cursor/unslop ~/.cursor/skills/
```

**This repo only**

```bash
git clone https://github.com/NoahWhiteson/unslop-cursor.git
mkdir -p .cursor/skills
cp -r unslop-cursor/unslop .cursor/skills/
```

Restart Cursor or start a new agent chat so the skill is picked up.

## Use

Ask in chat — the agent should load the skill when you mention unslopping or obvious slop:

```
unslop this dashboard
unslop the hero section
unslop https://example.com and keep our stack
unslop my landing page and make the story video
```

It audits first, proposes a direction, then fixes spacing → color → icons → copy → type → layout → details → visuals → motion. Heavy slop gets the full pass; light slop is polish mode; already-good screens get small suggestions only.

Optional **story video** (square, ~10s, morphing CSS steps): needs Playwright and ffmpeg — see `unslop/SKILL.md`.

Try the vibecoded before screens in [examples/](examples/) (`dashboard.html`, `hero.html`).

## Upstream

Behavior and credit follow the original repo. When you adapt or share the skill, keep attribution to Damir and link [heydamir/unslop](https://github.com/heydamir/unslop).

## License

[CC BY 4.0](LICENSE) — same as upstream.
