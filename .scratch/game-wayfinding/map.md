# Game Design Wayfinding Map

Label: wayfinder:map

## Destination

Produce a validated vertical-slice design brief for a solo, 2D, Godot-first RPG: define its player fantasy, core loop, combat, progression, world structure, and deliberately small first playable slice.

## Notes

Domain: a gameplay-first, loot-and-min-max RPG inspired by FFVII, FFX, FFXII, Terraria, Diablo, Forager, Rust, Skyrim, Dead Cells, and Hades. The target is a persistent solo character, with optional roguelite ideas only if they strengthen rather than replace RPG progression. Consult `grilling` and `domain-modeling` while resolving decisions. Use `CONTEXT.md` for canonical terms.

## Decisions so far

<!-- Closed decision tickets are indexed here. -->

- [Choose the 2D Spatial Grammar](issues/01-choose-2d-spatial-grammar.md) — Use side-on 2D; pair a static home region with expedition zones and progression-unlocked fixed stations.
- [Define Persistence and Run Structure](issues/02-define-persistence-and-run-structure.md) — Preserve the character and world; defeat resets only temporary expedition progress.
- [Choose the World Authorship Model](issues/03-choose-world-authorship-model.md) — Keep the home and introduction authored; assemble later expeditions from authored modules, then preserve and tier completed areas.
- [Define Combat and Build Identity](issues/04-define-combat-and-build-identity.md) — Use side-on real-time combat with free-mix weapons/materia and permanent use-based specialization mastery.
- [Design Use-Based Advancement](issues/05-design-use-based-advancement.md) — Pair modest overall-level growth and reassignable stats with encounter-earned, catch-up specialization mastery.
- [Define Core Loop and Goal Cadence](issues/06-define-core-loop-and-goal-cadence.md) — Prepare at home, secure at-risk valuables through expedition checkpoints, upgrade and clear objectives, then choose the next expedition or optional tiers.
- [Define Itemization, Stations, and Resource Economy](issues/07-define-itemization-stations-and-resource-economy.md) — Use simple randomized equipment, curated named items, three focused home stations, and distinct material, token, and currency roles.
- [Define Vertical-Slice Reward and Milestone Sequencing](issues/08-define-vertical-slice-reward-and-milestone-sequencing.md) — Teach crafting, combat, banking, traversal, materia, and boss rewards across a 20–30 minute authored expedition.
- [Define Vertical-Slice Success Criteria and Playtest Plan](issues/09-define-vertical-slice-success-criteria-and-playtest-plan.md) — Keep one focused expedition and judge it informally by whether friends understand its risks and enjoy replaying its build choices.
- [Define Vertical-Slice Setting and Audiovisual Direction](issues/10-define-vertical-slice-setting-and-audiovisual-direction.md) — Place the player in a warm fortified cave camp descending into cold, crystalline, ancient depths rendered in low-resolution pixel art.
- [Define Vertical-Slice Controls, Save, and Technical Boundaries](issues/11-define-vertical-slice-controls-save-and-technical-boundaries.md) — Ship an offline, gamepad-first PC slice with bounded actions, accessible settings, safe-point autosaves, and fixed 16:9 pixel-art framing.

## Not yet specified


## Out of scope

- Online multiplayer, co-op, and persistent shared worlds; this effort is solo-only.
- A full endgame/content model beyond optional expedition tiers; the destination is a bounded vertical-slice design brief.
- Shipping beyond a Godot-first PC prototype, including broader platform releases and production-scale technical architecture; these are later efforts.
