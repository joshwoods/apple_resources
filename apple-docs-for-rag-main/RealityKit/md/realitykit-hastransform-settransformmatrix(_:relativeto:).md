

- RealityKit
- HasTransform
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

## See Also

### Using a matrix

Transforming entities between RealityKit coordinate spaces

Move an entity between a volumetric window and an immersive space using coordinate space transformations.

func transformMatrix(relativeTo: Entity?) -> float4x4

Gets the 4 x 4 transform matrix of an entity relative to the given entity.

