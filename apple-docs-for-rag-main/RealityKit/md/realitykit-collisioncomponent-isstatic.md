

- RealityKit
- CollisionComponent
-  isStatic 

Instance Property

# isStatic

A Boolean value that indicates whether the collider is static.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var isStatic: Bool { get set }
```

## Discussion

When an object is static the physics engine recognizes that the object isn’t moving, which typically improves performance.

