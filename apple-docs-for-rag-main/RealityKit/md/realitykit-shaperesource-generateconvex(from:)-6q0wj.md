

- RealityKit
- ShapeResource
-  generateConvex(from:) 

Type Method

# generateConvex(from:)

Creates a convex shape from the given points.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateConvex(from points: [SIMD3]) -> ShapeResource
```

## Parameters 

`points`  

An array of 3D points that define the convex polyhedron. Keep the number of points small to avoid hurting performance.

## Return Value

The new shape.

## See Also

### Generating convex shapes

static func generateConvex(from: MeshResource) -> ShapeResource

Creates a convex shape from the given mesh.

