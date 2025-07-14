

- Model I/O
- MDLSubmesh
-  geometryType 

Instance Property

# geometryType

The type of geometric primitives described by the submesh’s index buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var geometryType: MDLGeometryType { get }
```

## Discussion

This property determines how the sequence of indices in the submesh’s index buffer should be interpreted for rendering. For example, if the geometry type is MDLGeometryType.triangles, each triangle to be rendered comes from an independent set of three indices, but if the geometry type is MDLGeometryType.triangleStrips, triangles to be rendered can come from overlapping sets of indices in the sequence. If the geometry type is MDLGeometryType.variableTopology, the topology property describes the non-uniform layout of the index buffer.

## See Also

### Working with a Submesh’s Index Buffer

var indexBuffer: any MDLMeshBuffer

An object that provides index data for the submesh.

var indexCount: Int

The number of indices in the submesh’s index buffer.

var indexType: MDLIndexBitDepth

The data type for each element in the submesh’s index buffer.

var topology: MDLSubmeshTopology?

A description of how the non-uniform layout of the submesh’s index buffer defines the shape of the mesh.

func indexBuffer(asIndexType: MDLIndexBitDepth) -> any MDLMeshBuffer

