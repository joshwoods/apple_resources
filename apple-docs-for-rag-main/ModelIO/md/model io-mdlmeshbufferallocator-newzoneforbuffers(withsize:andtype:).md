

- Model I/O
- MDLMeshBufferAllocator
-  newZoneForBuffers(withSize:andType:) 

Instance Method

# newZoneForBuffers(withSize:andType:)

Creates a zone large enough to fit the specified group of allocation sizes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newZoneForBuffers(
    withSize sizes: [NSNumber],
    andType types: [NSNumber]
) -> any MDLMeshBufferZone
```

**Required**

## Parameters 

`sizes`  

An array of integers, each the length in bytes of an allocation to be made later.

`types`  

An array of integers, each the MDLMeshBufferType value corresponding to an allocation described in the `sizes` array.

## Return Value

A new memory zone.

## Discussion

Objects implementing the MDLMeshBufferZone protocol describe a logical pool of memory for allocation of related buffers. The actual class of buffer zone objects vended by an allocator may be private.

This method creates a zone with enough capacity to allocate buffers with the sizes and types specified, taking into account any alignment restrictions necessary to use these buffers.

## See Also

### Allocating Mesh Buffers

func newZone(Int) -> any MDLMeshBufferZone

Creates a zone for related memory allocations.

**Required**

func newBuffer(Int, type: MDLMeshBufferType) -> any MDLMeshBuffer

Creates a new buffer of the specified length.

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

