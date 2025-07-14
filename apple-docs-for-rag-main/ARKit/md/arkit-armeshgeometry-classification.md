

- ARKit
- ARMeshGeometry
-  classification 

Instance Property

# classification

Classification for each face in the mesh.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var classification: ARGeometrySource? { get }
```

## Discussion

Each element of the array (ARGeometrySource) is a classification that corresponds to one face in the geometry. The `count` of this property represents the number of faces in the geometry. The default value at each index is `0`, –– the raw value for ARMeshClassification.none.

The following code demonstrates retrieving a classification for a particular face:

```
extension ARMeshGeometry {
    func classificationOf(faceWithIndex index: Int) -> ARMeshClassification {
        guard let classification = classification else { return .none }
        let classificationAddress = classification.buffer.contents().advanced(by: index)
        let classificationValue = Int(classificationAddress.assumingMemoryBound(to: UInt8.self).pointee)
        return ARMeshClassification(rawValue: classificationValue) ?? .none
    }
}
```

For a sample app that demonstrates classification, see Visualizing and interacting with a reconstructed scene.

## See Also

### Getting Geometry Information

enum ARMeshClassification

Enumeration of different classes of real-world objects that ARKit can identify.

var faces: ARGeometryElement

An object that contains a buffer of vertex indices of the geometry’s faces.

class ARGeometryElement

A container for index data, such as vertex indices of a face.

var normals: ARGeometrySource

Rays that define which direction is outside for each face.

