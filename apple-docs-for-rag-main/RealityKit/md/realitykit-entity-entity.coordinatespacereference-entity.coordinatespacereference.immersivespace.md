

- RealityKit
- Entity
- Entity.CoordinateSpaceReference
-  Entity.CoordinateSpaceReference.immersiveSpace 

Case

# Entity.CoordinateSpaceReference.immersiveSpace

A reference to an opened immersive space.

visionOS 2.0+

``` source
case immersiveSpace
```

## Discussion

You can use this enum case to get an entity’s relative transform to the immersive space:

```
let transformInImmersiveSpace = entity.transformMatrix(relativeTo: .immersiveSpace)
```

Note

If no immersive space is open, calling transformMatrix(relativeTo:) with the case `immersiveSpace` returns `nil`.

