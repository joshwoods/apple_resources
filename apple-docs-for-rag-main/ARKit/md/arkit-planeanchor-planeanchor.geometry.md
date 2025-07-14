

- ARKit
- PlaneAnchor
-  PlaneAnchor.Geometry 

Structure

# PlaneAnchor.Geometry

The geometry of a plane anchor.

visionOS 1.0+

``` source
struct Geometry
```

## Topics

### Inspecting plane geometry

var meshFaces: GeometryElement

The faces in the mesh that describes a plane.

var meshVertices: GeometrySource

The vertices in the mesh that describes a plane.

var extent: PlaneAnchor.Geometry.Extent

The size of a plane.

struct Extent

The size of a plane.

### Instance Properties

var description: String

A textual representation of this geometry.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Getting the shape of a plane anchor

var geometry: PlaneAnchor.Geometry

Get the geometry of the plane in the anchor’s coordinate system.

