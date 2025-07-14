

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- TransformAction
-  xformTarget 

Article

# xformTarget

A prim that provides the transform to which this action animates.

## Overview

To provide a transform, assign an Xformable prim to this property.

The prims in the list of affectedObjects animate from their current transform to the transform that this prim specifies. Include in the prim the transformational operations that implement the transform animation. For more information, see xformOp.

### Declaration

```
rel xformTarget
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

type

An option that controls the order in which the actions execute.

easeType

An option that describes the animation’s change in pace over time.

