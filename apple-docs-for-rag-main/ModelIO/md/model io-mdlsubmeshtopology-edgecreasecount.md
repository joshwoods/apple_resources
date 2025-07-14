

- Model I/O
- MDLSubmeshTopology
-  edgeCreaseCount 

Instance Property

# edgeCreaseCount

The number of entries in the edge creases buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var edgeCreaseCount: Int { get set }
```

## Discussion

The edgeCreases buffer contains this number of crease values. Because each edge is composed of two vertices, the edgeCreaseIndices buffer contains twice this number of vertex indices.

## See Also

### Identifying Creases

var edgeCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices that describe edges to be treated as creases during surface subdivision.

var edgeCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to edges during surface subdivision.

var vertexCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices to be treated as creases during surface subdivision.

var vertexCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to points during surface subdivision.

var vertexCreaseCount: Int

The number of entries in the vertex creases buffers.

