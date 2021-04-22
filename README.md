Stellaris Hackery
=================

General hackery and tinkering. This mod will not be gameplay-balanced or
necessarily even fun; its purpose is to be an exploration platform, and any
actually-viable mod ideas will be spun off into their own mods.

Installation:

Clone this repo into ~/.local/share/Paradox Interactive/Stellaris/mod (create
that directory if necessary), copy mod/Hackery/descriptor.mod into a new file
mod/Hackery.mod, and add this line at the bottom:

path="mod/Hackery"


- Console output? Works in some contexts, not others
- Console commands? Can't seem to create my own
- Add button to window??
- Change tooltip?
- Show total diplo weight across all galcom members
- Show your weight as a percentage
- Ultimately: Show your diplo dominance score.
  - Rank all other galcom members in descending weight order
  - Weight left = your weight
  - For each member:
    - If member's weight < weight left: Dominance++, subtract from weight left
    - Otherwise, dominance += weight left / member weight
  - If you are not the greatest member of the galcom, dominance < 1, and is how big you are compared to the biggest
  - If you are equal weightiest, dominance = 1
  - Otherwise, it's the number of other empires that have to band together to outvote you.
  - Show dominance as "out of N" where N is number of galcom members
  - What happens if you call in favours? How will that change your dominance? Can I even see that?
