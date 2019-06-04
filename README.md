# UnrealEngine--WaypointGenerator
A blueprint module for visualizing navigational paths in Unreal Engine v4.22. As of v1.2, the system also supports path updates at runtime based on player/objective locations (https://www.youtube.com/watch?v=oNj44ra3ss8).

**Design Process:** https://unrealpossibilities.blogspot.com/2018/06/unreal-engine-experiments-waypoint.html

**Preview video:** https://www.youtube.com/watch?v=LgHrSM3WEiw

**Integration Tutorial:** https://www.youtube.com/watch?v=2XQupaI4gbQ

(Content in this project may only be used in Unreal Engine projects as per the Unreal Engine 4 EULA)

## Notes:
- Path points are generated using UE4's navmesh, while Instanced Static Meshes are used to visualize Waypoints.
- The Instanced Static Meshes used for path visualization are reused during each update cycle, adding new ones and removing excess instances only when necessary. Even so, it basically comes down to the addition of at most one instanced mesh per several update cycles, while all existing instances just require transform updates.
