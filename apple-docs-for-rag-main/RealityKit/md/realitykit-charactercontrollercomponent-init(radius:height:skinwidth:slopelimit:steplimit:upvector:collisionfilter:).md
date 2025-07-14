

- RealityKit
- CharacterControllerComponent
-  init(radius:height:skinWidth:slopeLimit:stepLimit:upVector:collisionFilter:) 

Initializer

# init(radius:height:skinWidth:slopeLimit:stepLimit:upVector:collisionFilter:)

Creates a character controller component using specified values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    radius: Float,
    height: Float,
    skinWidth: Float = defaultSkinWidth,
    slopeLimit: Float = defaultSlopeLimit,
    stepLimit: Float = defaultStepLimit,
    upVector: SIMD3 = defaultUpVector,
    collisionFilter: CollisionFilter = .default
)
```

## See Also

### Creating a character controller component

init()

Creates a character controller component using default values.

