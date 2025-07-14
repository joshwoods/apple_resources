

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
-  MeshResource.ShapeExtrusionOptions.ExtrusionMethod 

Enumeration

# MeshResource.ShapeExtrusionOptions.ExtrusionMethod

The options that determine the way in which to extrude a swept shape in 3D.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ExtrusionMethod
```

## Topics

### Enumeration Cases

case linear(depth: Float)

Extrudes the shape with a linear extrusion in Z by the desired depth.

case tracePositions([SIMD3&lt;Float>])

Extrudes the shape by sweeping it along a piecewise-linear curve.

case traceTransforms([simd_float4x4])

Extrudes the shape by sweeping it along a piecewise-linear curve.

## Relationships

### Conforms To

- Sendable

## See Also

### 2D path extrusion for 3D mesh creation

struct ShapeExtrusionOptions

A type that determines the extrusion, chamfering, and material assignment of an extruded shape.

struct MaterialAssignment

A type that determines the material assignments for each part of an extruded shape.

enum ChamferMode

Determines which part of the extrusion to chamfer.

enum CurveStrokeResolution

Designates the resolution at which a smooth curve is discretized.

