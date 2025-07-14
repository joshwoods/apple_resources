

- Model I/O
- MDLMesh
-  init(meshBySubdividingMesh:submeshIndex:subdivisionLevels:allocator:) 

Initializer

# init(meshBySubdividingMesh:submeshIndex:subdivisionLevels:allocator:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    meshBySubdividingMesh mesh: MDLMesh,
    submeshIndex: Int32,
    subdivisionLevels: UInt32,
    allocator: (any MDLMeshBufferAllocator)?
)
```

## See Also

### Creating a Custom Mesh

init(vertexBuffer: any MDLMeshBuffer, vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh from a single vertex buffer with the specified parameters.

init(vertexBuffers: [any MDLMeshBuffer], vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh by unifying vertex data from multiple sources with the specified parameters.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

class func newSubdividedMesh(MDLMesh, submeshIndex: Int, subdivisionLevels: Int) -> Self?

Creates a new mesh by subdividing the specified mesh.

