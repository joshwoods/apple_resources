

- ARKit
- ARMeshGeometry
-  normals 

Instance Property

# normals

Rays that define which direction is outside for each face.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var normals: ARGeometrySource { get }
```

## See Also

### Getting Geometry Information

var classification: ARGeometrySource?

Classification for each face in the mesh.

enum ARMeshClassification

Enumeration of different classes of real-world objects that ARKit can identify.

var faces: ARGeometryElement

An object that contains a buffer of vertex indices of the geometry’s faces.

class ARGeometryElement

A container for index data, such as vertex indices of a face.

