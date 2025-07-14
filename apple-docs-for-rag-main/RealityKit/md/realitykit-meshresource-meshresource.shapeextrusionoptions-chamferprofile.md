

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
-  chamferProfile 

Instance Property

# chamferProfile

A path that determines the cross-sectional contour of each chamfered edge.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+visionOS 2.0+

``` source
var chamferProfile: Path? { get set }
```

## Discussion

Note

If the chamfer profile is `nil`, a circular profile is used.

The chamfer profile needs to satisfy the following conditions:

- The path is nonempty.

- The first point on the path is at (0, 0) and the last point is at (1, 1).

- The value of x along the profile either increases or stays the same. In other words, the profile curve may not wrap back on itself.

To learn more about SwiftUI’s Path structure, see Drawing paths and shapes.

