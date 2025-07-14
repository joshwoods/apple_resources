

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- OrbitAction
-  axis 

Article

# axis

A vector that describes the axis of rotation.

## Overview

The object spins in a plane perpendicular to the value of this property. To reverse a spin direction, invert the value of this property. The default value points positively in the y-direction.

### Declaration

```
uniform vector3d axis = (0.0, 1.0, 0.0)
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

alignToPath

An option that controls the prim’s orientation as it revolves.

