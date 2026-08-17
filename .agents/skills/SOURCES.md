# Installed project skills

| Skills | Upstream | License |
| --- | --- | --- |
| `godot-gdscript-patterns` | [wshobson/agents](https://github.com/wshobson/agents) | MIT |
| `godot-master` | [thedivergentai/gd-agentic-skills](https://github.com/thedivergentai/gd-agentic-skills) | LGPL-3.0 |
| `godot-2d-movement`, `godot-animation`, `godot-physics`, `godot-resources`, `godot-tilemap`, `godot-ui-control` | [gamedev-skills/awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) | Apache-2.0 |

## Blender skills

Installed a curated core from [roble3/cc-blender-skill](https://github.com/roble3/cc-blender-skill) (MIT):

- `blender-modeling`, `blender-materials`, `blender-uv-texturing`
- `blender-animation`, `blender-lighting`, `blender-cameras`
- `blender-rendering`, `blender-export`
- `text-to-blender`, `blender-pro-workflow`, `blender-skill-harmonizer` (orchestration and shared backend references)

Copied complete skill directories, including their scripts and references, without local modifications. The pinned upstream commit and SHA-256 of each installed file are in [`blender-sources.lock.json`](blender-sources.lock.json); the license is [`LICENSE-cc-blender-skill`](LICENSE-cc-blender-skill).

Selection evidence at installation: GitHub reported 109 stars; skills.sh reported approximately 1.9K modeling installs, 1.3K materials installs, and 1.1K each for animation, lighting, rendering, export, and pro-workflow. UV texturing (938), cameras (938), text-to-blender (889), and harmonizer (712) were included for pipeline coverage and shared dependencies. Popularity is not proof of correctness: these are community-authored recipes, not official Blender guidance. Reviewed the core skill instructions; did not execute every bundled script or validate every recipe on the installed Blender version.

The web-oriented `blender-web-pipeline` was evaluated but not restored: this project uses Godot, not Three.js. Existing Godot skills remain unchanged.

See [`../BLENDER.md`](../BLENDER.md) for project-specific usage and backend limitations.

## Existing Godot installation

The Godot skills were installed with `npx skills` into this project. Their exact source paths and content hashes are recorded in the root [`skills-lock.json`](../../skills-lock.json).
