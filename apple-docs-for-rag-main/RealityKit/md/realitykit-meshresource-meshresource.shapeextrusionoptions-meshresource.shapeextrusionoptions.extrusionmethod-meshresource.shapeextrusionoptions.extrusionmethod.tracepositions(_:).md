

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
- MeshResource.ShapeExtrusionOptions.ExtrusionMethod
-  MeshResource.ShapeExtrusionOptions.ExtrusionMethod.tracePositions(\_:) 

Case

# MeshResource.ShapeExtrusionOptions.ExtrusionMethod.tracePositions(\_:)

Extrudes the shape by sweeping it along a piecewise-linear curve.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case tracePositions([SIMD3])
```

## Discussion

The curve is defined as the set of line segments For each edge in the provided curve, the swept shape (e.g. the 2D path provided in `MeshResource(extruding: Path)`, or text) will be instantiated at the edge’s endpoints. Each instance of the swept shape will be joined together by a strip of geometry.

The positions are traced in such a way as to avoid twist in the generated 3D shape. When possible, the local y-axis of the swept (2D) shape will be aligned with the y-axis of the generated 3D shape.

For example, extrude a rounded square along the z-axis, while zig-zagging in the y-axis:

```
// Positions in a zig-zag pattern.
let positions: [SIMD3] = [
    [0,    0,   0],
    [0, -0.1, 0.2],
    [0,    0, 0.4],
    [0, -0.1, 0.6]
]

var extrusionOptions = ShapeExtrusionOptions()
extrusionOptions.extrusionMethod = .tracePositions(positions)
```

