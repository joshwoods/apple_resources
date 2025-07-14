

- RealityKit
- MeshResource
-  MeshResource.ShapeExtrusionOptions 

Structure

# MeshResource.ShapeExtrusionOptions

A type that determines the extrusion, chamfering, and material assignment of an extruded shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ShapeExtrusionOptions
```

## Topics

### Structures

struct MaterialAssignment

A type that determines the material assignments for each part of an extruded shape.

### Initializers

init()

Creates the shape extrusion options with default values.

### Instance Properties

var boundaryResolution: MeshResource.ShapeExtrusionOptions.CurveStrokeResolution

Resolution of the shape.

var chamferMode: MeshResource.ShapeExtrusionOptions.ChamferMode

Determines if the front, back or both sides should be chamfered.

var chamferProfile: Path?

A path that determines the cross-sectional contour of each chamfered edge.

var chamferRadius: Float

The width or depth, in meters, of each chamfered edge.

var chamferResolution: MeshResource.ShapeExtrusionOptions.CurveStrokeResolution

Resolution of the chamfer curve.

var extrusionMethod: MeshResource.ShapeExtrusionOptions.ExtrusionMethod

Specifies the extrusion type applied to the swept shape in 3D space.

var materialAssignment: MeshResource.ShapeExtrusionOptions.MaterialAssignment

Determines the material assignments for each part of an extruded shape.

### Enumerations

enum ChamferMode

Determines which part of the extrusion to chamfer.

enum CurveStrokeResolution

Designates the resolution at which a smooth curve is discretized.

enum ExtrusionMethod

The options that determine the way in which to extrude a swept shape in 3D.

## Relationships

### Conforms To

- Sendable

## See Also

### 2D path extrusion for 3D mesh creation

struct MaterialAssignment

A type that determines the material assignments for each part of an extruded shape.

enum ChamferMode

Determines which part of the extrusion to chamfer.

enum CurveStrokeResolution

Designates the resolution at which a smooth curve is discretized.

enum ExtrusionMethod

The options that determine the way in which to extrude a swept shape in 3D.

