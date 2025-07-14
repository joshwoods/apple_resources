

- Model I/O
- MDLMeshBufferZone
-  capacity 

Instance Property

# capacity

The data capacity of the zone, in bytes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var capacity: Int { get }
```

**Required**

## Discussion

You specify the capacity of a zone when creating it with the newZone(_:) method of a concrete class implementing the MDLMeshBufferAllocator protocol.

## See Also

### Inspecting a Zone

var allocator: any MDLMeshBufferAllocator

The allocator object that created the zone.

**Required**

