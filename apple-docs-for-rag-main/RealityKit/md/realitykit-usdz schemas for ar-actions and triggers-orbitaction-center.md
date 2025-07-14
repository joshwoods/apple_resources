

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- OrbitAction
-  center 

Article

# center

A prim around which the affected objects orbit.

## Overview

Assign this property a prim not contained by affectedObjects.

To reside at an arbitrary location in its parent’s coordinate space, a prim needs the translation component of a transform. Therefore, assign this property an Xformable prim.

### Declaration

```
rel center
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

revolutions

The number of rotations to complete.

axis

A vector that describes the axis of rotation.

alignToPath

An option that controls the prim’s orientation as it revolves.

