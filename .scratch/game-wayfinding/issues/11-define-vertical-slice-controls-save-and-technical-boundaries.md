# Define Vertical-Slice Controls, Save, and Technical Boundaries

Type: grilling
Status: resolved
Assignee: Cody

## Question

For the solo, PC-first Godot vertical slice, what input scheme, accessibility baseline, save behavior, and technical boundaries are required to make the 20–30 minute side-on expedition comfortably playable and safely persistent—without prematurely designing future platform support or production architecture?

## Answer

Design the slice gamepad-first, with keyboard support implemented through an input abstraction. The initial action set is movement, jump, basic attack, universal dodge/dash, interact, and one equipped materia ability. Weapon specials and their meter remain designed but are not implemented in the slice.

Provide remappable controls, separate master/music/SFX volume controls, readable scalable text, and reduced screen shake. Use one named local save slot. Autosave at the home region and when banking at an expedition checkpoint; after quitting, restore the player to that last safe location, preserving only progress committed there.

Target a fixed 16:9 pixel-art internal resolution that scales cleanly to desktop windows and fullscreen. Unsupported aspect ratios are letterboxed or pillarboxed. The slice is an offline, PC-first Godot build; future platforms and production-scale architecture are deliberately deferred.
