

- Metal
-  MTLSizeAndAlign 

Structure

# MTLSizeAndAlign

The size and alignment of a resource, in bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLSizeAndAlign
```

## Topics

### Accessing the Size and Alignment

var size: Int

The size of a resource, in bytes.

var align: Int

The alignment of a resource, in bytes.

### Creating Instances

init()

Creates a default instance.

init(size: Int, align: Int)

Creates a new instance initialized to the given values.

## Relationships

### Conforms To

- BitwiseCopyable
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

enum MTLHeapType

The options you use to choose the heap type.

