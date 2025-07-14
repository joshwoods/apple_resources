

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- LookAtCameraAction
-  upVector 

Article

# upVector

A vector around which the runtime rotates the object.

## Overview

This property defines the axis around which the runtime rotates the target to create the effect of a prim looking at the user. Normally, an asset defines this value to match the stage’s upAxis. The default value points positively in the y-direction.

### Declaration

```
uniform vector3d upVector = (0.0, 1.0, 0.0)
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

front

A vector that’s perpendicular to, and points outward from, the object’s face.

