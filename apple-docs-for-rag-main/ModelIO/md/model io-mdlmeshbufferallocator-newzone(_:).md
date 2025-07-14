

- Model I/O
- MDLMeshBufferAllocator
-  newZone(\_:) 

Instance Method

# newZone(\_:)

Creates a zone for related memory allocations.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newZone(_ capacity: Int) -> any MDLMeshBufferZone
```

**Required**

## Parameters 

`capacity`  

The capacity of the zone to be created.

## Return Value

A new memory zone.

## Discussion

Objects implementing the MDLMeshBufferZone protocol describe a logical pool of memory for allocation of related buffers. The actual class of buffer zone objects vended by an allocator may be private.

## See Also

### Allocating Mesh Buffers

func newZoneForBuffers(withSize: [NSNumber], andType: [NSNumber]) -> any MDLMeshBufferZone

Creates a zone large enough to fit the specified group of allocation sizes.

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

