

- Model I/O
- MDLSubmesh
-  init(name:indexBuffer:indexCount:indexType:geometryType:material:) 

Initializer

# init(name:indexBuffer:indexCount:indexType:geometryType:material:)

Initializes a named submesh with an index buffer and the specified properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    name: String,
    indexBuffer: any MDLMeshBuffer,
    indexCount: Int,
    indexType: MDLIndexBitDepth,
    geometryType: MDLGeometryType,
    material: MDLMaterial?
)
```

## Parameters 

`name`  

A descriptive name for the submesh. This property is not used in rendering, but can be useful in debugging.

`indexBuffer`  

An object that provides index data for the submesh.

`indexCount`  

The number of indices in the index buffer.

`indexType`  

The data type of each index in the index buffer.

`geometryType`  

The type of geometric primitives described by the index buffer.

`material`  

A description of the intended surface appearance for rendering the submesh.

## Return Value

A new submesh object.

## Discussion

Typically, a submesh is imported from an asset file as a member of a MDLMesh object, but you can also use this method to create a submesh programmatically.

## See Also

### Creating a Submesh

init(indexBuffer: any MDLMeshBuffer, indexCount: Int, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType, material: MDLMaterial?)

Initializes a submesh with an index buffer and the specified properties.

init(name: String, indexBuffer: any MDLMeshBuffer, indexCount: Int, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType, material: MDLMaterial?, topology: MDLSubmeshTopology?)

Initializes a named submesh with a specific topology.

init?(mdlSubmesh: MDLSubmesh, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType)

Initializes a submesh by copying or converting another submesh.

