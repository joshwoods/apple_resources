

- RealityKit
- MeshDescriptor
-  MeshDescriptor.Primitives 

Enumeration

# MeshDescriptor.Primitives

Indicates which primitive shape type a mesh applies to its vertex indices.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum Primitives
```

## Topics

### Enumeration Cases

case polygons([UInt8], [UInt32])

Defines one or more triangles and quadrilaterals with two separate arrays of indices.

case triangles([UInt32])

Defines one or more triangles with an integer array of indices.

case trianglesAndQuads(triangles: [UInt32], quads: [UInt32])

Defines separate arrays for triangle and quad indices.

## See Also

### Static meshes

struct MeshDescriptor

Defines a 3D mesh’s structure and data.

enum Materials

