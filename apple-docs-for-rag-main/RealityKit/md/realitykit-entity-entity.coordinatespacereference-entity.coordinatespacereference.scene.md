

- RealityKit
- Entity
- Entity.CoordinateSpaceReference
-  Entity.CoordinateSpaceReference.scene 

Case

# Entity.CoordinateSpaceReference.scene

A reference to an entity’s parent window scene.

visionOS 2.0+

``` source
case scene
```

## Discussion

You can use this enum case to get an entity’s relative transform in its parented window scene:

```
let transformInWindowSpace = windowEntity.transformMatrix(relativeTo: .scene)
```

Note

If an entity is parented under an **immersive space**, calling transformMatrix(relativeTo:) with the case `scene` returns `nil`.

