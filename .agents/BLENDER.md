# Blender asset workflow

Godot remains the game engine. Blender is an optional asset-authoring tool, not a replacement for Godot or a reason to restore Three.js skills.

## Fit to this game

The current brief in `CONTEXT.md` targets a side-on, 2D pixel-art game. Use Blender for authored props, equipment icons, environment pieces, or animation frames rendered to PNG. A 3D render is not automatically convincing pixel art: inspect silhouettes, palette, edge treatment, and readability at the actual in-game resolution. Do not change the game's art direction without approval.

For sprite work:

1. Block out geometry and lock an orthographic side-view camera.
2. Choose a consistent pixels-per-unit scale, framing, lighting, and transparent RGBA background.
3. Render a small proof at the intended sprite size; inspect it visually before detailing.
4. Render animation frames with identical framing and pivot placement; pack a spritesheet if needed.
5. Import into Godot with nearest filtering for pixel art, and verify scale, animation timing, and readability in-game.

For explicitly requested 3D assets, prefer glTF 2.0/GLB for Godot rather than the upstream suite's generic FBX advice. Bake unsupported procedural materials into textures, retain editable `.blend` sources, and validate materials, scale, orientation, skeletons, and animation clips inside Godot. Generic upstream size/polycount limits are examples, not this game's requirements.

## Skills and execution

The core Blender skills live in `.agents/skills/`; source and integrity information is in `SOURCES.md` and `blender-sources.lock.json` there. Start with the relevant domain skill; use `blender-pro-workflow` for multi-stage work.

Blender was found at `/Applications/Blender.app/Contents/MacOS/Blender` (reported version 5.2.1 LTS at installation). This is a machine-local path, not a portable project dependency.

The upstream orchestrator and backend instructions expect Blender MCP. Installing skills does **not** install or configure that backend, and no MCP server/add-on configuration was changed in this task. Before interactive MCP work, verify tool availability and the intended open scene using `text-to-blender/references/mcp-backends.md`.

For a separately chosen headless workflow, the domain skills' `bpy` recipes can be adapted into a Python file and run directly with Blender, without MCP:

```sh
/Applications/Blender.app/Contents/MacOS/Blender --background --factory-startup --python /absolute/path/to/asset_script.py
```

Run headless scripts only against a new scene or an explicitly selected input file. Do not reset an existing world, delete geometry, overwrite source files, or change Blender preferences just because a generic upstream recipe suggests it. Check operators/properties against the installed Blender API: some recipes use older APIs. Inspect actual rendered images before claiming visual success.

Only the core suite is installed. Upstream mentions optional reconstruction, reference-calibration, and quality-loop skills that are not included; do not assume they exist. Inspect available skill folders before following such a handoff. Shared backend references and core orchestration dependencies are included.
