

- Model I/O
- MDLSubmeshTopology
-  edgeCreaseIndices 

Instance Property

# edgeCreaseIndices

A buffer containing vertex indices that describe edges to be treated as creases during surface subdivision.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var edgeCreaseIndices: (any MDLMeshBuffer)? { get set }
```

## Discussion

Each pair of entries in this buffer identifies an edge, between two connected vertices in the submesh, that is to be treated as a crease during surface subdivision. The buffer is sparse, containing only those vertex indices to be treated as creases. The corresponding entry in the edgeCreases buffer provides a sharpness value for the crease.

Because the number of entries in this buffer is likely to be different than the number of entries in any other vertex buffer, it shouldn’t be interleaved with other data in the mesh.

## See Also

### Identifying Creases

var edgeCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to edges during surface subdivision.

var edgeCreaseCount: Int

The number of entries in the edge creases buffers.

var vertexCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices to be treated as creases during surface subdivision.

var vertexCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to points during surface subdivision.

var vertexCreaseCount: Int

The number of entries in the vertex creases buffers.

