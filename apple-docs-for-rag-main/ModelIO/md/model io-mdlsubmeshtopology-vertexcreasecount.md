

- Model I/O
- MDLSubmeshTopology
-  vertexCreaseCount 

Instance Property

# vertexCreaseCount

The number of entries in the vertex creases buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var vertexCreaseCount: Int { get set }
```

## See Also

### Identifying Creases

var edgeCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices that describe edges to be treated as creases during surface subdivision.

var edgeCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to edges during surface subdivision.

var edgeCreaseCount: Int

The number of entries in the edge creases buffers.

var vertexCreaseIndices: (any MDLMeshBuffer)?

A buffer containing vertex indices to be treated as creases during surface subdivision.

var vertexCreases: (any MDLMeshBuffer)?

A buffer containing sharpness values to be applied to points during surface subdivision.

