# UnrealEngine--WaypointGenerator
A blueprint module for visualizing navigational paths in Unreal Engine v4.22.

**Preview Video:** https://www.youtube.com/watch?v=LgHrSM3WEiw

**Design Process:** https://unrealpossibilities.blogspot.com/2018/06/unreal-engine-experiments-waypoint.html

(Content in this project may only be used in Unreal Engine projects as per the Unreal Engine 4 EULA)

## Notes:
- Path points generated through UE4's nav mesh queries.
- Instanced Static Meshes used to display waypoints.

## Limitations:
- Does not support parallel alignment (pitch/roll) of waypoint meshes along inclined surfaces.
- Does not support dynamic path updates based on continuously changing player/objective locations.
