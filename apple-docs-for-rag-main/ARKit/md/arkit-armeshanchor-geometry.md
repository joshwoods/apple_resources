

- ARKit
- ARMeshAnchor
-  geometry 

Instance Property

# geometry

3D information about the mesh such as its shape and classifications.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var geometry: ARMeshGeometry { get }
```

## Discussion

Contains the anchor’s portion of mesh data that, with any other mesh anchors in the AR session, collectively reconstruct the scene around the user. The mesh anchor records this data in it’s own coordinate system.

## See Also

### Accessing the Mesh

class ARMeshGeometry

Mesh information stored in an efficient, array-based format.

