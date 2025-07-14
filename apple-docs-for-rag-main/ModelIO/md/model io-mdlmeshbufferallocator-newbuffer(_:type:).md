

- Model I/O
- MDLMeshBufferAllocator
-  newBuffer(\_:type:) 

Instance Method

# newBuffer(\_:type:)

Creates a new buffer of the specified length.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newBuffer(
    _ length: Int,
    type: MDLMeshBufferType
) -> any MDLMeshBuffer
```

**Required**

## Parameters 

`length`  

The size, in bytes, of the buffer to create.

`type`  

Use MDLMeshBufferType.vertex to create a buffer for a mesh’s vertex attribute data, or MDLMeshBufferType.index to create a buffer for a submesh’s index data.

## Return Value

A new memory buffer for mesh data.

## Discussion

The concrete class implementing this protocol determines the initial contents of the buffer and the memory pool from which the buffer is allocated. To provide a hint that multiple related allocations should share the same pool of memory, use the newBuffer(from:length:type:) method instead.

## See Also

### Allocating Mesh Buffers

func newZone(Int) -> any MDLMeshBufferZone

Creates a zone for related memory allocations.

**Required**

func newZoneForBuffers(withSize: [NSNumber], andType: [NSNumber]) -> any MDLMeshBufferZone

Creates a zone large enough to fit the specified group of allocation sizes.

**Required**

func newBuffer(from: (any MDLMeshBufferZone)?, length: Int, type: MDLMeshBufferType) -> (any MDLMeshBuffer)?

Creates a new buffer of the specified length in the specified zone.

**Required**

func newBuffer(with: Data, type: MDLMeshBufferType) -> any MDLMeshBuffer

Creates a new buffer containing the specified data.

**Required**

func newBuffer(from: (any MDLMeshBufferZone)?, data: Data, type: MDLMeshBufferType) -> (any MDLMeshBuffer)?

Creates a new buffer containing the specified data in the specified zone.

**Required**

