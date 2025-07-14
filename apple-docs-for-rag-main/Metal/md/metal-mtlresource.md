

- Metal
-  MTLResource 

Protocol

# MTLResource

An allocation of memory accessible to a GPU.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLResource : MTLAllocation
```

## Mentioned in 

Choosing a Resource Storage Mode for Intel and AMD GPUs

Synchronizing a Managed Resource in macOS

## Overview

Important

Don’t implement this protocol yourself. Create resources by calling methods on MTLDevice, MTLBuffer, or MTLTexture.

When you execute commands on the GPU, those commands can only affect memory allocated as MTLResource objects. Only the MTLDevice that created these resources can modify them. Different resource types have different uses. The most common resource types are buffers (MTLBuffer), which are linear allocations of memory, and textures (MTLTexture), which hold structured image data.

## Topics

### Identifying the Resource

var device: any MTLDevice

The device object that created the resource.

**Required**

var label: String?

A string that identifies the resource.

**Required**

### Reading Memory and Storage Properties

var cpuCacheMode: MTLCPUCacheMode

The CPU cache mode that defines the CPU mapping of the resource.

**Required**

var storageMode: MTLStorageMode

The location and access permissions of the resource.

**Required**

var hazardTrackingMode: MTLHazardTrackingMode

A mode that determines whether Metal tracks and synchronizes resource access.

**Required**

var resourceOptions: MTLResourceOptions

The storage mode, CPU cache mode, and hazard tracking mode of the resource.

**Required**

enum MTLCPUCacheMode

Options for the CPU cache mode that define the CPU mapping of the resource.

enum MTLStorageMode

Options for the memory location and access permissions for a resource.

enum MTLHazardTrackingMode

The options you use to specify the hazard tracking mode.

### Setting the Purgeable State of the Resource

func setPurgeableState(MTLPurgeableState) -> MTLPurgeableState

Specifies or queries the resource’s purgeable state.

**Required**

enum MTLPurgeableState

The purgeable state of the resource.

### Managing Heap Resources

var heapOffset: Int

The distance, in bytes, from the beginning of the heap to the first byte of the resource, if you allocated the resource on a heap.

**Required**

var heap: (any MTLHeap)?

The heap on which the resource is allocated, if any.

**Required**

func makeAliasable()

Allows future heap resource allocations to alias against the resource’s memory, reusing it.

**Required**

func isAliasable() -> Bool

A Boolean value that indicates whether future heap resource allocations may alias against the resource’s memory.

**Required**

### Querying the Allocated Size

var allocatedSize: Int

The size of the resource, in bytes.

**Required**

## Relationships

### Inherits From

- MTLAllocation
- NSObjectProtocol

### Inherited By

- MTLAccelerationStructure
- MTLBuffer
- MTLIndirectCommandBuffer
- MTLIntersectionFunctionTable
- MTLTexture
- MTLVisibleFunctionTable

## See Also

### Common Resource Functionality

protocol MTLAllocation

A memory allocation from a Metal GPU device, such as a memory heap, texture, or data buffer.

struct MTLResourceOptions

Optional arguments used to set the behavior of a resource.

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

struct MTLResourceID

