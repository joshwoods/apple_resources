

- RealityKit
- ShapeResource
-  generateCapsule(height:radius:) 

Type Method

# generateCapsule(height:radius:)

Creates a capsule shape with the specified height and radius.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateCapsule(
    height: Float,
    radius: Float
) -> ShapeResource
```

## Parameters 

`height`  

The height of the capsule including the spherical caps in meters, measured along the local y-axis.

`radius`  

The radius of the capsule in meters.

## Return Value

The new capsule.

## Discussion

Note

Collision shape extents that fall below 2mm are forced to be 2mm in size - this includes, entities with negative scale values.

