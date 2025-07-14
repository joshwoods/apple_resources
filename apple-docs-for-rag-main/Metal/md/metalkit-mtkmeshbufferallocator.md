

- MetalKit
-  MTKMeshBufferAllocator 

Class

# MTKMeshBufferAllocator

An interface for allocating a MetalKit buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MTKMeshBufferAllocator
```

## Topics

### Initialization

init(device: any MTLDevice)

Initializes a new allocator object.

### Device

var device: any MTLDevice

The device used to create Metal objects.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLMeshBufferAllocator
- NSObjectProtocol

## See Also

### Model Handling

class MTKMesh

A container for the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKMeshBuffer

A buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKSubmesh

A container for the index data of a Model I/O submesh, suitable for use in a Metal app.

Conversion Functions

Convert between Metal and Model I/O vertex representations.

Model Errors

Learn about errors thrown by model handling methods.

