

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
-  MeshResource.ShapeExtrusionOptions.MaterialAssignment 

Structure

# MeshResource.ShapeExtrusionOptions.MaterialAssignment

A type that determines the material assignments for each part of an extruded shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct MaterialAssignment
```

## Topics

### Initializers

init(assignAll: UInt32)

Creates a material assignment structure that assigns the same material to all faces.

init(front: UInt32, back: UInt32, extrusion: UInt32, frontChamfer: UInt32, backChamfer: UInt32)

Creates a material assignment structure with options for each side of an extruded shape.

## Relationships

### Conforms To

- Sendable

## See Also

### 2D path extrusion for 3D mesh creation

struct ShapeExtrusionOptions

A type that determines the extrusion, chamfering, and material assignment of an extruded shape.

enum ChamferMode

Determines which part of the extrusion to chamfer.

enum CurveStrokeResolution

Designates the resolution at which a smooth curve is discretized.

enum ExtrusionMethod

The options that determine the way in which to extrude a swept shape in 3D.

