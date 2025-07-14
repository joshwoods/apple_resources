

- RealityKit
- LowLevelMesh
- LowLevelMesh.Descriptor
-  vertexBufferCount 

Instance Property

# vertexBufferCount

The number of buffers this descriptor uses.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var vertexBufferCount: Int { get }
```

## Discussion

This value derives from the maximum `bufferIndex` each layout specifies in vertexLayouts.

## See Also

### Defining the descriptor’s contents

var indexType: MTLIndexType

The data type of the indices that the index buffer stores.

var vertexAttributes: [LowLevelMesh.Attribute]

An array that describes the vertex input attributes to a vertex function.

var vertexLayouts: [LowLevelMesh.Layout]

The list of layouts.

