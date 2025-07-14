

- RealityKit
- ShapeResource
-  generateConvex(from:) 

Type Method

# generateConvex(from:)

Creates a convex shape from the given mesh.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
nonisolated
static func generateConvex(from mesh: MeshResource) async throws -> ShapeResource
```

## Parameters 

`mesh`  

A mesh with the shape of the convex polyhedron. Use meshes with a small number of vertices to avoid hurting performance.

## Return Value

The new shape, defined by the convex hull of the vertices in `mesh`.

## Discussion

Throws

Will throw an error if `mesh` does not define a nonempty convex volume. For example, will fail if all the vertices in `mesh` are coplanar.

