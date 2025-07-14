

- ARKit
- PlaneAnchor
- PlaneAnchor.Geometry
-  PlaneAnchor.Geometry.Extent 

Structure

# PlaneAnchor.Geometry.Extent

The size of a plane.

visionOS 1.0+

``` source
struct Extent
```

## Topics

### Inspecting a plane extent

var width: Float

The width of a plane.

var height: Float

The height of a plane.

var anchorFromExtentTransform: simd_float4x4

The transform from the plane extent to the plane anchor’s coordinate system.

### Instance Properties

var description: String

A textual representation of this extent.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Inspecting plane geometry

var meshFaces: GeometryElement

The faces in the mesh that describes a plane.

var meshVertices: GeometrySource

The vertices in the mesh that describes a plane.

var extent: PlaneAnchor.Geometry.Extent

The size of a plane.

