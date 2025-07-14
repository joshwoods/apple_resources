

- Model I/O
- MDLMeshBufferZone
-  allocator 

Instance Property

# allocator

The allocator object that created the zone.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var allocator: any MDLMeshBufferAllocator { get }
```

**Required**

## Discussion

Use the newZone(_:) method of a concrete class implementing the MDLMeshBufferAllocator protocol to create a zone.

## See Also

### Inspecting a Zone

var capacity: Int

The data capacity of the zone, in bytes.

**Required**

