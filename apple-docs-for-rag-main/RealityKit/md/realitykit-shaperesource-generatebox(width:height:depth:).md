

- RealityKit
- ShapeResource
-  generateBox(width:height:depth:) 

Type Method

# generateBox(width:height:depth:)

Creates a box shape with the specified dimensions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateBox(
    width: Float,
    height: Float,
    depth: Float
) -> ShapeResource
```

## Parameters 

`width`  

The extent of the box along the x-axis in meters.

`height`  

The extent of the box along the y-axis in meters.

`depth`  

The extent of the box along the z-axis in meters.

## Return Value

The new box centered at the local origin and aligned with the local axes.

## Discussion

Note

Collision shape extents that fall below 2mm are forced to be 2mm in size - this includes, entities with negative scale values.

## See Also

### Generating boxes

static func generateBox(size: SIMD3&lt;Float>) -> ShapeResource

Creates a box shape with the specified extent.

