

- RealityKit
- ShapeResource
-  generateConvex(from:) 

Type Method

# generateConvex(from:)

Creates a convex shape from the given mesh.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateConvex(from mesh: MeshResource) -> ShapeResource
```

## Parameters 

`mesh`  

A mesh with the shape of the convex polyhedron. Use meshes with a small number of vertices to avoid hurting performance.

## Return Value

The new shape.

## See Also

### Generating convex shapes

static func generateConvex(from: [SIMD3&lt;Float>]) -> ShapeResource

Creates a convex shape from the given points.

