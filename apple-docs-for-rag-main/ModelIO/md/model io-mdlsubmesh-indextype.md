

- Model I/O
- MDLSubmesh
-  indexType 

Instance Property

# indexType

The data type for each element in the submesh’s index buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var indexType: MDLIndexBitDepth { get }
```

## Discussion

For optimum performance, an index buffer should generally use the smallest possible data type to fit its number of indices.

## See Also

### Working with a Submesh’s Index Buffer

var indexBuffer: any MDLMeshBuffer

An object that provides index data for the submesh.

var indexCount: Int

The number of indices in the submesh’s index buffer.

var geometryType: MDLGeometryType

The type of geometric primitives described by the submesh’s index buffer.

var topology: MDLSubmeshTopology?

A description of how the non-uniform layout of the submesh’s index buffer defines the shape of the mesh.

func indexBuffer(asIndexType: MDLIndexBitDepth) -> any MDLMeshBuffer

