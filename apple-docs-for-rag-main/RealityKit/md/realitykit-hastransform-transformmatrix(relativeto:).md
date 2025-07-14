

- RealityKit
- HasTransform
-  transformMatrix(relativeTo:) 

Instance Method

# transformMatrix(relativeTo:)

Gets the 4 x 4 transform matrix of an entity relative to the given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func transformMatrix(relativeTo referenceEntity: Entity?) -> float4x4
```

## Parameters 

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The transform of the entity relative to `referenceEntity`.

## See Also

### Using a matrix

Transforming entities between RealityKit coordinate spaces

Move an entity between a volumetric window and an immersive space using coordinate space transformations.

func setTransformMatrix(float4x4, relativeTo: Entity?)

Sets the transform of the entity relative to the given reference entity using a 4x4 matrix representation.

