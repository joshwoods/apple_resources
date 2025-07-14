

- ARKit
- ARMeshGeometry
-  faces 

Instance Property

# faces

An object that contains a buffer of vertex indices of the geometry’s faces.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var faces: ARGeometryElement { get }
```

## Discussion

Each element of the buffer-based array is a three-index combination that forms a unique triangle, or *face*. The index refers to that vertex’s position in the vertices array. The count of this property represents the number of faces.

The following code demonstrates getting the vertices of a particular face:

```
extension ARMeshGeometry {
    func vertexIndicesOf(faceWithIndex index: Int) -> [Int] {
        let indicesPerFace = faces.indexCountPerPrimitive
        let facesPointer = faces.buffer.contents()
        var vertexIndices = [Int]()
        for offset in 0...size)
            vertexIndices.append(Int(vertexIndexAddress.assumingMemoryBound(to: UInt32.self).pointee))
        }
        return vertexIndices
    }
}
```

## See Also

### Getting Geometry Information

var classification: ARGeometrySource?

Classification for each face in the mesh.

enum ARMeshClassification

Enumeration of different classes of real-world objects that ARKit can identify.

class ARGeometryElement

A container for index data, such as vertex indices of a face.

var normals: ARGeometrySource

Rays that define which direction is outside for each face.

