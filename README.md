# UnrealEngine--WaypointGenerator
A blueprint module for visualizing navigational paths in Unreal Engine v4.22.

**Design Process:** https://unrealpossibilities.blogspot.com/2018/06/unreal-engine-experiments-waypoint.html

(Content in this project may only be used in Unreal Engine projects as per the Unreal Engine 4 EULA)

## Notes:
- The Instanced Static Meshes used for path visualization are reused during each update cycle, adding new ones and removing excess instances only when necessary. Even so, it basically comes down to the addition of at most one instanced mesh per several update cycles, while all existing instances just require transform updates.
