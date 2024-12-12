# Superliminal recreation in Unreal 5

Trying to recreate the main mechanics in Superliminal in Blueprints using Unreal Engine 5.

Superliminal's force perspective mechanic is an interesting feature where selected objects appear locked to the player's view even when moving or rotating the camera. However, the cube is actually being scaled in the actual game world in order to maintain its size from the player's perspective.

# How to use

**Controls:**
- Movement: Arrow keys move the player
- Jump: space key jumps
- rotate camera: move mouse to move camera view
- Select/deselect object: left mouse button selects or deselect an object

**How to try it out:**

1. Add a `BP_SelectableCube` to the scene, look at it, then select it with the left mouse button to lock it to the player's view. 
2. Move the player or player's camera to move the cube and change its size.
3. Click again to release the cube. It will retain its size and interact with gravity again.

**Features:**
- `BP_FirstPersonPlayer` is the player that is capable of moveing and selecting objects.
- `BAC_SelectableComponent` is a component you attach to game objects to mark them as selectable.
- `BP_SelectableCube` is a complete working example of a selectable object.

