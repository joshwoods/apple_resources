

- RealityKit
- PhysicsBodyComponent
-  isTranslationLocked 

Instance Property

# isTranslationLocked

A tuple of Boolean values that you use to lock the position of the physics body along any of the three axes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var isTranslationLocked: (x: Bool, y: Bool, z: Bool)
```

## Discussion

You can restrict movement of the body along one or more axes by setting the corresponding item in the tuple to `true`. For example, if you set the `x` and the `z` items in the tuple to `true`, then the body can move only along the y-axis. By default, movement isn’t restricted.

## See Also

### Locking movement

var isRotationLocked: (x: Bool, y: Bool, z: Bool)

A tuple of Boolean values that you use to lock rotation of the physics body around any of the three axes.

