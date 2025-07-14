

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
-  MeshResource.ShapeExtrusionOptions.ChamferMode 

Enumeration

# MeshResource.ShapeExtrusionOptions.ChamferMode

Determines which part of the extrusion to chamfer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ChamferMode
```

## Topics

### Operators

static func == (MeshResource.ShapeExtrusionOptions.ChamferMode, MeshResource.ShapeExtrusionOptions.ChamferMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case back

Only chamfer the back of the extrusion.

case both

Chamfer both the front and the back of the extrusion.

case front

Only chamfer the front of the extrusion.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### 2D path extrusion for 3D mesh creation

struct ShapeExtrusionOptions

A type that determines the extrusion, chamfering, and material assignment of an extruded shape.

struct MaterialAssignment

A type that determines the material assignments for each part of an extruded shape.

enum CurveStrokeResolution

Designates the resolution at which a smooth curve is discretized.

enum ExtrusionMethod

The options that determine the way in which to extrude a swept shape in 3D.

