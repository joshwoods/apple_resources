

- RealityKit
- Entity
-  transformMatrix(relativeTo:) 

Instance Method

# transformMatrix(relativeTo:)

Returns the 4 x 4 transform matrix of an entity relative to the given coordinate space.

visionOS 2.0+

``` source
@MainActor @preconcurrency
func transformMatrix(relativeTo referenceSpace: Entity.CoordinateSpaceReference) -> float4x4?
```

## Parameters 

`referenceSpace`  

The coordinate space that defines a frame of reference.

## Return Value

The transform of the entity relative to `referenceSpace`, or `nil` when the given coordinate space is not applicable to the given entity.

## Discussion

This method overloads transformMatrix(relativeTo:).

## See Also

### Positioning entities in space

protocol HasTransform

An interface that enables manipulating the scale, rotation, and translation of an entity.

struct Transform

A component that defines the scale, rotation, and translation of an entity.

enum CoordinateSpaceReference

Defines the coordinate space reference for transform conversion.

enum ForwardDirection

Defines the forward direction for an entity.

