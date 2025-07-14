

- Model I/O
- MDLSubmeshTopology
-  edgeCreases 

Instance Property

# edgeCreases

A buffer containing sharpness values to be applied to edges during surface subdivision.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var edgeCreases: (any MDLMeshBuffer)? { get set }
```

## Discussion

Each entry in this buffer corresponds to a pair of entries in the edgeCreaseIndices buffer that identifies a crease. The value of each entry determines the amount of smoothing to apply to the crease during surface subdivision—a value of zero completely smooths out the edge, and a value of one leaves the edge completely sharp.

Because the number of entries in this buffer is likely to be different than the number of entries in any other vertex buffer, it shouldn’t be interleaved with other data in the mesh.

## See Also

### Identifying Creases

var edgeCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices that describe edges to be treated as creases during surface subdivision.

var edgeCreaseCount: Int

The number of entries in the edge creases buffers.

var vertexCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices to be treated as creases during surface subdivision.

var vertexCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to points during surface subdivision.

var vertexCreaseCount: Int

The number of entries in the vertex creases buffers.

