

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
- MeshResource.ShapeExtrusionOptions.ExtrusionMethod
-  MeshResource.ShapeExtrusionOptions.ExtrusionMethod.traceTransforms(\_:) 

Case

# MeshResource.ShapeExtrusionOptions.ExtrusionMethod.traceTransforms(\_:)

Extrudes the shape by sweeping it along a piecewise-linear curve.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case traceTransforms([simd_float4x4])
```

## Discussion

The swept shape (e.g. the 2D path provided in `MeshResource(extruding: Path)`, or text) is instantiated at each of the provided transforms. Each instance is joined together by a strip of geometry. You can specify a different rotation of the swept shape for each point on the curve with `traceTransforms`.

For example, extrude a rounded square along the z-axis while zig-zagging in the y-axis, using the default rotation throughout. This creates a mesh where the swept shapes have the same orientation.

```
// Positions in a zig-zag pattern.
let positions: [SIMD3] = [
    [0,    0,   0],
    [0, -0.1, 0.2],
    [0,    0, 0.4],
    [0, -0.1, 0.6]
]

var extrusionOptions = ShapeExtrusionOptions()
extrusionOptions.extrusionMethod = .traceTransforms(
    positions.map { position in
        Transform(translation: position).matrix
    }
)
```

You can also add a rotation for each point in the collection. For example, use the index to rotate the angle by `.pi / 6` in the z-axis for each position.

```
extrusionOptions.extrusionMethod = .traceTransforms(
    positions.enumerated().map { index, position in
        Transform(
            rotation: simd_quatf(
                // Increase the angle depending on index.
                angle: Float(index) * .pi / 6, axis: [0, 0, 1]
            ),
            translation: position
        ).matrix
    }
)
```

