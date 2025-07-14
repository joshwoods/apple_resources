

- RealityKit
- LowLevelMesh
- LowLevelMesh.Part
-  init(indexOffset:indexCount:topology:materialIndex:bounds:) 

Initializer

# init(indexOffset:indexCount:topology:materialIndex:bounds:)

Creates a low-level mesh part.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    indexOffset: Int = 0,
    indexCount: Int = 0,
    topology: MTLPrimitiveType = .triangle,
    materialIndex: Int = 0,
    bounds: BoundingBox
)
```

## Parameters 

`indexOffset`  

The offset, in bytes, of the first index.

`indexCount`  

The number of indices to use for this part.

`topology`  

The geometric primitive to use when rendering this part.

`materialIndex`  

The material index this part associates with.

`bounds`  

The model-space bounding box of the part.

