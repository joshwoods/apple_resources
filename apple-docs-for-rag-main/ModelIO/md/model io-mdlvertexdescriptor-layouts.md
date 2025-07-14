

- Model I/O
- MDLVertexDescriptor
-  layouts 

Instance Property

# layouts

The list of vertex buffer layouts described by the vertex descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var layouts: NSMutableArray { get set }
```

## Discussion

A MDLVertexBufferLayout object describes the layout of data in one of the vertex buffers of a of a MDLMesh object.

For meshes whose vertex data is split into multiple vertex buffers (a *structure of arrays* design), the order of objects in this array reflects the order of buffers in the mesh’s vertexBuffers array, which in turn parallels the order of vertex attributes in the descriptor’s attributes array. If a mesh contains interleaved data in a single vertex buffer (an *array of structures* design), the descriptor contains only one MDLVertexBufferLayout object, which describes the offset between entries for consecutive vertices in the buffer.

## See Also

### Working with Vertex Buffer Layouts

func setPackedStrides()

Sets the stride for each vertex layout to the minimum value to pack vertex data together in a single buffer.

