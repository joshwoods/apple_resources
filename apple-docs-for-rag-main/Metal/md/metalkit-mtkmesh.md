

- MetalKit
-  MTKMesh 

Class

# MTKMesh

A container for the vertex data of a Model I/O mesh, suitable for use in a Metal app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MTKMesh
```

## Topics

### Initialization

init(mesh: MDLMesh, device: any MTLDevice) throws

Initializes a MetalKit mesh and its submeshes from a Model I/O mesh.

### Loading Meshes from an Asset

class func newMeshes(asset: MDLAsset, device: any MTLDevice) throws -> (modelIOMeshes: [MDLMesh], metalKitMeshes: [MTKMesh])

### Submeshes

var submeshes: [MTKSubmesh]

An array of submeshes containing index buffers referencing the mesh vertices.

### Vertex Properties

var vertexBuffers: [MTKMeshBuffer]

An array of buffers in which mesh vertex data resides.

var vertexCount: Int

The number of vertices in the vertex buffers.

var vertexDescriptor: MDLVertexDescriptor

A Model I/O vertex descriptor specifying the data layout in the vertex buffers.

### Identifying Properties

var name: String

The name of the mesh.

### Constants

Mesh Error Handling

Strings used when handling NSError messages returned from a mesh initialization method.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Model Handling

class MTKMeshBuffer

A buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKMeshBufferAllocator

An interface for allocating a MetalKit buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKSubmesh

A container for the index data of a Model I/O submesh, suitable for use in a Metal app.

Conversion Functions

Convert between Metal and Model I/O vertex representations.

Model Errors

Learn about errors thrown by model handling methods.

