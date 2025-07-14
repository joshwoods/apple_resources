

- RealityKit
- Entity
-  setTransformMatrix(\_:relativeTo:) 

Instance Method

# setTransformMatrix(\_:relativeTo:)

Sets the transform of the entity relative to the given reference entity using a 4x4 matrix representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func setTransformMatrix(
    _ transform: float4x4,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`transform`  

A 4x4 transform matrix, given relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Discussion

The Transform component can’t represent all transforms that a general 4x4 matrix can represent. Setting a transform using a 4x4 matrix is therefore a lossy event that might result in certain transformations, like shear, being dropped.

