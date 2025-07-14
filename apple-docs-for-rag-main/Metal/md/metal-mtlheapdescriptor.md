

- Metal
-  MTLHeapDescriptor 

Class

# MTLHeapDescriptor

A configuration that customizes the behavior for a Metal memory heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MTLHeapDescriptor
```

## Mentioned in 

Creating Sparse Heaps and Sparse Textures

## Overview

Create an MTLHeap by configuring an MTLHeapDescriptor instance’s properties and passing it to the makeHeap(descriptor:) method of an MTLDevice.

Each new heap inherits the descriptor’s configuration as you create it, which means you can modify and reuse a descriptor to create other heaps.

## Topics

### Configuring a Heap

var type: MTLHeapType

The memory placement strategy for any resources you allocate from the heaps you create with this descriptor.

var storageMode: MTLStorageMode

The storage mode for the heaps you create with this descriptor.

var cpuCacheMode: MTLCPUCacheMode

The CPU cache behavior for any resources you allocate from the heaps you create with this descriptor.

var hazardTrackingMode: MTLHazardTrackingMode

The hazard tracking behavior for any resources you allocate from the heaps you create with this descriptor.

var resourceOptions: MTLResourceOptions

The combined behavior for any resources you allocate from the heaps you create with this descriptor.

var size: Int

The total amount of memory, in bytes, for the heaps you create with this descriptor.

var sparsePageSize: MTLSparsePageSize

The page size for any resources you allocate from the heaps you create with this descriptor.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

enum MTLHeapType

The options you use to choose the heap type.

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

