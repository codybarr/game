# Choose the 2D Spatial Grammar

Type: grilling
Status: resolved

## Question

Which 2D spatial grammar should organize play—side-on platforming, top-down movement, isometric (a diagonal top-down view that makes 2D scenes appear to have depth), or another form—and what does that choice enable for exploration, combat, gathering, and building?

## Answer

Use a side-on 2D spatial grammar. It was chosen over top-down because the initial combat should be easier to implement. The player will work from a persistent home region into bounded expedition zones. For the vertical slice, terrain is static: there is no mining, destructibility, or free-form building. The home region instead gains fixed, interactable crafting and magic stations as progression unlocks.
