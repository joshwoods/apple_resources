

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- OrbitAction
-  alignToPath 

Article

# alignToPath

An option that controls the prim’s orientation as it revolves.

## Overview

The default value is `false`, in which the object maintains its orientation as it travels along the orbit path. Set a value of `true` to reorient the object to face the center as it orbits.

### Declaration

```
uniform bool alignToPath = false
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

center

A prim around which the affected objects orbit.

duration

The amount of time that the objects face the camera.

revolutions

The number of rotations to complete.

axis

A vector that describes the axis of rotation.

