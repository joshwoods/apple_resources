

- Model I/O
- MDLMeshBuffer
-  zone 

Instance Property

# zone

The memory pool from which the buffer was created.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var zone: any MDLMeshBufferZone { get }
```

**Required**

## Discussion

Use the newBuffer(from:data:type:) or newBuffer(from:length:type:) method of an allocator to reserve memory in a shared pool for multiple related buffers.

## See Also

### Inspecting a Buffer

var allocator: any MDLMeshBufferAllocator

The allocator object that created the buffer.

**Required**

var type: MDLMeshBufferType

The type of data contained in a buffer.

**Required**

