

- Model I/O
- MDLMesh
-  init(vertexBuffers:vertexCount:descriptor:submeshes:) 

Initializer

# init(vertexBuffers:vertexCount:descriptor:submeshes:)

Creates a mesh by unifying vertex data from multiple sources with the specified parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    vertexBuffers: [any MDLMeshBuffer],
    vertexCount: Int,
    descriptor: MDLVertexDescriptor,
    submeshes: [MDLSubmesh]
)
```

## Parameters 

`vertexBuffers`  

An array of objects, each of which provides a separate source of vertex information for the mesh.

`vertexCount`  

The number of vertices in the mesh.

`descriptor`  

An object describing the type and layout of vertex attribute data in the vertex buffers.

`submeshes`  

An array of submesh objects, each of which provides index buffer and material information describing how some or all of the mesh’s vertex data is to be rendered.

## Return Value

A new mesh object.

## Discussion

Use this initializer to create a mesh from vertex data that describes separate vertex attributes in separate arrays with matching indices (a structure of arrays).

## See Also

### Creating a Custom Mesh

init(vertexBuffer: any MDLMeshBuffer, vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh from a single vertex buffer with the specified parameters.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

class func newSubdividedMesh(MDLMesh, submeshIndex: Int, subdivisionLevels: Int) -> Self?

Creates a new mesh by subdividing the specified mesh.

init(meshBySubdividingMesh: MDLMesh, submeshIndex: Int32, subdivisionLevels: UInt32, allocator: (any MDLMeshBufferAllocator)?)

