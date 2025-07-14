

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- TransformAction
-  easeType 

Article

# easeType

An option that describes the animation’s change in pace over time.

## Overview

The default type is `none`, which is synonymous with linear timing.

### Ease Types

`none`  
Paces the action at a constant rate.

`in`  
Paces the action slower at the beginning.

`out`  
Paces the action slower at the end.

`inout`  
Paces the action slower at the beginning and end.

### Declaration

```
uniform token easeType = "none"
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

xformTarget

A prim that provides the transform to which this action animates.

duration

The amount of time that the objects face the camera.

type

An option that controls the order in which the actions execute.

