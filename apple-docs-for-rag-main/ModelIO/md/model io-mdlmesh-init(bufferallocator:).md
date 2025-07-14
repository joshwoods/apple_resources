

- Model I/O
- MDLMesh
-  init(bufferAllocator:) 

Initializer

# init(bufferAllocator:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(bufferAllocator: (any MDLMeshBufferAllocator)?)
```

## See Also

### Creating a Custom Mesh

init(vertexBuffer: any MDLMeshBuffer, vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh from a single vertex buffer with the specified parameters.

init(vertexBuffers: [any MDLMeshBuffer], vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh by unifying vertex data from multiple sources with the specified parameters.

class func newSubdividedMesh(MDLMesh, submeshIndex: Int, subdivisionLevels: Int) -> Self?

Creates a new mesh by subdividing the specified mesh.

init(meshBySubdividingMesh: MDLMesh, submeshIndex: Int32, subdivisionLevels: UInt32, allocator: (any MDLMeshBufferAllocator)?)

