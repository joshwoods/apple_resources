

- RealityKit
- LowLevelMesh
- LowLevelMesh.Descriptor
-  maxVertexBufferCount 

Type Property

# maxVertexBufferCount

The maximum number of separate buffers the system supports.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static let maxVertexBufferCount: Int
```

## Discussion

For optimal performance, most applications use one buffer.

## See Also

### Defining the descriptor’s limits

var vertexCapacity: Int

The number of vertices to allocate space for.

var indexCapacity: Int

The number of indices to allocate space for.

