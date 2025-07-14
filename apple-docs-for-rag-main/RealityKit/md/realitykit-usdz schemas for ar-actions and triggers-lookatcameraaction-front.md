

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- LookAtCameraAction
-  front 

Article

# front

A vector that’s perpendicular to, and points outward from, the object’s face.

## Overview

From the value of this property, the runtime calculates how much to spin the target object about the upVector. This property is in local space, and so it’s relative to the target object’s coordinate space. The default value faces positively in the x-direction.

### Declaration

```
uniform vector3d front = (1.0, 0.0, 0.0)
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

upVector

A vector around which the runtime rotates the object.

