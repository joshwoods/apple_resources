

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- EmphasizeAction
-  style 

Article

# style

An option that implements different kinds of animation timing.

## Overview

The default value is `basic`.

### Styles

`basic`  
Animates with steady motion.

`playful`  
Animates with whimsical motion.

`wild`  
Animates with sporadic motion.

### Declaration

```
uniform token style = "basic" (
    allowedTokens = ["basic", "playful", "wild"]
)
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

motionType

An option that determines how the action displays or hides a prim.

