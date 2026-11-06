# Heat-Marked House

Design concept for the Caltech D2D FIRES project (Eaton Fire). By Lynn Liu.

An interactive sketch of a stucco house that is heated by a nearby fire but does not burn down. Pick what is burning, drag it closer or farther, and see how much radiant heat reaches each wall, how that heat moves through the wall layer by layer, and how an inspection record (CAL FIRE DINS classes) can miss damage hidden behind the stucco.

## Open it

Open `index.html` in a browser. It is one self-contained file; it needs an internet connection to load Three.js r128 from a CDN.

## What is in the page

- **3D house**: drag the fire, click a wall to see the temperature through it, double-click to open the wall layers. The north wall is drawn as a section with its layers peeled back (depth ×4).
- **Right panel**: temperature through the wall at the marked point, layer by layer.
- **Bottom panel**: what an inspector would likely record vs what is inside the wall; second tab shows how long contaminants stay and how long insurance pays for living elsewhere.
- **Timeline**: the Eaton Fire from January 2025 to 2027, by category (emergency, cleanup, insurance, research, public health and law).

## Data and assumptions

- Radiant heat: flames treated as a black-body panel (σT⁴) with a numerical view factor to each wall patch.
- Heat through the wall: 1D finite-volume conduction with typical material values (stucco, building paper, plywood, glass-fibre insulation or wood stud, gypsum).
- Flame size, flame temperature, the fire curve and the wall build-up are **assumed typical values**, not measurements of a real house.
- Stucco color stages (pink, grey, buff) and wood char/ignition thresholds come from engineering literature.
- Durations of contaminants and insurance rules come from published studies and California law, not from the model.

This is a design concept, not a damage assessment. Sources are listed at the bottom of the page.
