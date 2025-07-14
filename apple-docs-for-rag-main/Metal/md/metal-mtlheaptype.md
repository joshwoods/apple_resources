

- Metal
-  MTLHeapType 

Enumeration

# MTLHeapType

The options you use to choose the heap type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum MTLHeapType
```

## Topics

### Specifying the Heap Type

case automatic

A heap that automatically places new resource allocations.

case placement

The app controls placement of resources on the heap.

case sparse

The heap contains sparse texture tiles.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Resource Memory Allocation and Management

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

protocol MTLHeap

A memory pool from which you can suballocate resources.

class MTLHeapDescriptor

A configuration that customizes the behavior for a Metal memory heap.

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

