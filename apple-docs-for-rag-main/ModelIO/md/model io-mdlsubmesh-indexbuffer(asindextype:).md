

- Model I/O
- MDLSubmesh
-  indexBuffer(asIndexType:) 

Instance Method

# indexBuffer(asIndexType:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func indexBuffer(asIndexType indexType: MDLIndexBitDepth) -> any MDLMeshBuffer
```

## See Also

### Working with a Submesh’s Index Buffer

var indexBuffer: any MDLMeshBuffer

An object that provides index data for the submesh.

var indexCount: Int

The number of indices in the submesh’s index buffer.

var indexType: MDLIndexBitDepth

The data type for each element in the submesh’s index buffer.

var geometryType: MDLGeometryType

The type of geometric primitives described by the submesh’s index buffer.

var topology: MDLSubmeshTopology?

A description of how the non-uniform layout of the submesh’s index buffer defines the shape of the mesh.

