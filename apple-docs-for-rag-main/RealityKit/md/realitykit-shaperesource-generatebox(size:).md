

- RealityKit
- ShapeResource
-  generateBox(size:) 

Type Method

# generateBox(size:)

Creates a box shape with the specified extent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateBox(size: SIMD3) -> ShapeResource
```

## Parameters 

`size`  

The box extent in meters along the local axes.

## Return Value

The new box centered at the local origin and aligned with the local axes.

## Discussion

Note

Collision shape extents that fall below 2mm are forced to be 2mm in size - this includes, entities with negative scale values.

## See Also

### Generating boxes

static func generateBox(width: Float, height: Float, depth: Float) -> ShapeResource

Creates a box shape with the specified dimensions.

