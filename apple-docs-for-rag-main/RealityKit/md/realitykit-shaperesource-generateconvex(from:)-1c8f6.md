

- RealityKit
- ShapeResource
-  generateConvex(from:) 

Type Method

# generateConvex(from:)

Creates a convex shape from the given points asynchronously.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
nonisolated
static func generateConvex(from points: [SIMD3]) async throws -> ShapeResource
```

## Parameters 

`points`  

An array of 3D points that define the convex polyhedron. Keep the number of points small to avoid hurting performance.

## Return Value

A new ShapeResource object defined by the convex hull of `points`.

## Discussion

Throws

Will throw an error if `points` do not define a nonempty convex volume. For example, will fail if all of the points in `points` are coplanar.

