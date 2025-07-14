

- RealityKit
- LowLevelMesh
- LowLevelMesh.Descriptor
-  vertexLayouts 

Instance Property

# vertexLayouts

The list of layouts.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var vertexLayouts: [LowLevelMesh.Layout] { get set }
```

## Discussion

You assign a layout for each vertex attribute with layoutIndex.

## See Also

### Defining the descriptor’s contents

var indexType: MTLIndexType

The data type of the indices that the index buffer stores.

var vertexAttributes: [LowLevelMesh.Attribute]

An array that describes the vertex input attributes to a vertex function.

var vertexBufferCount: Int

The number of buffers this descriptor uses.

