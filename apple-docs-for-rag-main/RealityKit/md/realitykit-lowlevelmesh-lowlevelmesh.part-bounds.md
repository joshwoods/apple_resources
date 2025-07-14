

- RealityKit
- LowLevelMesh
- LowLevelMesh.Part
-  bounds 

Instance Property

# bounds

The model-space bounding box of this part.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var bounds: BoundingBox
```

## Discussion

RealityKit uses this bounding box for culling the mesh against the active camera.

Take care to maintain the bounds of each mesh part so that it completely contains the part’s geometry. Otherwise, RealityKit may not render your meshes correctly.

## See Also

### Describing a low-level mesh part

var indexOffset: Int

The offset, in bytes, of the first index.

var indexCount: Int

The number of indices to use for this part.

var topology: MTLPrimitiveType

The geometric primitive to use when rendering this part.

var materialIndex: Int

The material index this part associates with.

