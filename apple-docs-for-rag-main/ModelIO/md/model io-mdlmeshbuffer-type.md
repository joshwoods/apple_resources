

- Model I/O
- MDLMeshBuffer
-  type 

Instance Property

# type

The type of data contained in a buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var type: MDLMeshBufferType { get }
```

**Required**

## Discussion

A buffer can contain per-vertex data for one or more vertex attributes of a MDLMesh object (MDLMeshBufferType.vertex), or index data for a MDLSubmesh object (MDLMeshBufferType.index).

## See Also

### Inspecting a Buffer

var allocator: any MDLMeshBufferAllocator

The allocator object that created the buffer.

**Required**

var zone: any MDLMeshBufferZone

The memory pool from which the buffer was created.

**Required**

