

- ARKit
- MeshAnchor
-  MeshAnchor.Geometry 

Structure

# MeshAnchor.Geometry

The shapes that make up a mesh anchor.

visionOS 1.0+

``` source
struct Geometry
```

## Topics

### Inspecting mesh geometry

var faces: GeometryElement

The faces of the mesh.

var vertices: GeometrySource

The vertices of the mesh.

var normals: GeometrySource

The normals of the mesh.

var classifications: GeometrySource?

The classification of each face in the mesh.

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

### Getting mesh information

var originFromAnchorTransform: simd_float4x4

The location and orientation of a mesh in world space.

var geometry: MeshAnchor.Geometry

The shape of a mesh anchor.

enum MeshClassification

The kinds of classification a face of a mesh can have.

