

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
-  MeshResource.ShapeExtrusionOptions.CurveStrokeResolution 

Enumeration

# MeshResource.ShapeExtrusionOptions.CurveStrokeResolution

Designates the resolution at which a smooth curve is discretized.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum CurveStrokeResolution
```

## Topics

### Enumeration Cases

case uniformSegmentsPerSpan(segmentCount: Int)

For each span of the curve, generates a uniform number of segments.

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

enum ExtrusionMethod

The options that determine the way in which to extrude a swept shape in 3D.

