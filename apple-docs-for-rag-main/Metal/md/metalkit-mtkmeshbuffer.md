

- MetalKit
-  MTKMeshBuffer 

Class

# MTKMeshBuffer

A buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MTKMeshBuffer
```

## Topics

### Originating Objects

var allocator: MTKMeshBufferAllocator

The allocator object used to create this mesh buffer.

var type: MDLMeshBufferType

The type of data contained in the originating Model I/O buffer.

### Metal Buffer Properties

var buffer: any MTLBuffer

The Metal buffer backing all vertex and index data.

var length: Int

The logical size of the Metal buffer, in bytes.

var offset: Int

The byte offset of the data within the Metal buffer.

### Instance Methods

func zone() -> (any MDLMeshBufferZone)?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLMeshBuffer
- MDLNamed
- NSCopying
- NSObjectProtocol

## See Also

### Model Handling

class MTKMesh

A container for the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKMeshBufferAllocator

An interface for allocating a MetalKit buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKSubmesh

A container for the index data of a Model I/O submesh, suitable for use in a Metal app.

Conversion Functions

Convert between Metal and Model I/O vertex representations.

Model Errors

Learn about errors thrown by model handling methods.

