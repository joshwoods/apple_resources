

- Metal
-  MTLHeap 

Protocol

# MTLHeap

A memory pool from which you can suballocate resources.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
protocol MTLHeap : MTLAllocation
```

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

Improving CPU Performance by Using Argument Buffers

Reducing the Memory Footprint of Metal Apps

Creating Sparse Heaps and Sparse Textures

## Overview

Don’t implement this protocol yourself; instead, to create a heap, configure a MTLHeapDescriptor object and call the makeHeap(descriptor:) method of a MTLDevice object.

You suballocate resources from a heap and make them *aliasable* or *non-aliasable*. A sub-allocated resource is non-aliased by default, preventing future resources allocated from the heap from using its memory. Resources are *aliased* when they share the same memory allocation on a heap.

All resources sub-allocated from the same heap share the same storage mode and CPU cache mode. You can make heaps purgeable, but not the resources allocated from the heap; they can only reflect the heap’s purgeability state.

## Topics

### Identifying the Heap

var device: any MTLDevice

The device object that created the heap.

**Required**

var label: String?

A string that identifies the heap.

**Required**

### Querying Heap Properties

var type: MTLHeapType

The heap’s type.

**Required**

var storageMode: MTLStorageMode

The heap’s storage mode.

**Required**

var cpuCacheMode: MTLCPUCacheMode

The heap’s CPU cache mode.

**Required**

var hazardTrackingMode: MTLHazardTrackingMode

The heap’s hazard tracking mode.

**Required**

var resourceOptions: MTLResourceOptions

The options for resources created by the heap.

**Required**

var size: Int

The total size of the heap, in bytes.

**Required**

var usedSize: Int

The size of all resources currently in the heap, in bytes.

**Required**

var currentAllocatedSize: Int

The size, in bytes, of the current heap allocation.

**Required**

func maxAvailableSize(alignment: Int) -> Int

The maximum size of a resource, in bytes, that can be currently allocated from the heap.

**Required**

enum MTLHeapType

The options you use to choose the heap type.

### Setting the Purgeable State of the Resource

func setPurgeableState(MTLPurgeableState) -> MTLPurgeableState

Sets the purgeable state of the heap.

**Required**

### Creating Resources on the Heap

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture on the heap.

**Required**

func makeBuffer(length: Int, options: MTLResourceOptions, offset: Int) -> (any MTLBuffer)?

Creates a buffer at a specified offset on the heap.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, offset: Int) -> (any MTLTexture)?

Creates a texture at a specified offset on the heap.

**Required**

### Instance Methods

func makeAccelerationStructure(descriptor: MTLAccelerationStructureDescriptor) -> (any MTLAccelerationStructure)?

**Required**

func makeAccelerationStructure(descriptor: MTLAccelerationStructureDescriptor, offset: Int) -> (any MTLAccelerationStructure)?

**Required**

func makeAccelerationStructure(size: Int) -> (any MTLAccelerationStructure)?

**Required**

func makeAccelerationStructure(size: Int, offset: Int) -> (any MTLAccelerationStructure)?

**Required**

## Relationships

### Inherits From

- MTLAllocation
- NSObjectProtocol

## See Also

### Resource Memory Allocation and Management

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

class MTLHeapDescriptor

A configuration that customizes the behavior for a Metal memory heap.

enum MTLHeapType

The options you use to choose the heap type.

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

