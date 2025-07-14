

- Model I/O
- MDLMeshBufferAllocator
-  newBuffer(from:length:type:) 

Instance Method

# newBuffer(from:length:type:)

Creates a new buffer of the specified length in the specified zone.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newBuffer(
    from zone: (any MDLMeshBufferZone)?,
    length: Int,
    type: MDLMeshBufferType
) -> (any MDLMeshBuffer)?
```

**Required**

## Parameters 

`zone`  

A pool of memory for related allocations, as returned by the newZone(_:) method.

`length`  

The size, in bytes, of the buffer to create.

`type`  

Use MDLMeshBufferType.vertex to create a buffer for a mesh’s vertex attribute data, or MDLMeshBufferType.index to create a buffer for a submesh’s index data.

## Return Value

A new memory buffer for mesh data.

## Discussion

Use this method when making multiple related allocations that should share the same memory pool.

The concrete class implementing this protocol determines the initial contents of the buffer.

## See Also

### Allocating Mesh Buffers

func newZone(Int) -> any MDLMeshBufferZone

Creates a zone for related memory allocations.

**Required**

func newZoneForBuffers(withSize: [NSNumber], andType: [NSNumber]) -> any MDLMeshBufferZone

Creates a zone large enough to fit the specified group of allocation sizes.

**Required**

func newBuffer(Int, type: MDLMeshBufferType) -> any MDLMeshBuffer

Creates a new buffer of the specified length.

**Required**

func newBuffer(with: Data, type: MDLMeshBufferType) -> any MDLMeshBuffer

Creates a new buffer containing the specified data.

**Required**

func newBuffer(from: (any MDLMeshBufferZone)?, data: Data, type: MDLMeshBufferType) -> (any MDLMeshBuffer)?

Creates a new buffer containing the specified data in the specified zone.

**Required**

