

- Metal
-  MTLAllocation 

Protocol

# MTLAllocation

A memory allocation from a Metal GPU device, such as a memory heap, texture, or data buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol MTLAllocation : NSObjectProtocol
```

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Overview

Types that conform to MTLAllocation, including MTLBuffer, MTLTexture, and MTLHeap, have underlying memory. You make their memory *resident*, or GPU-accessible, by adding an allocation to an MTLResidencySet or calling the appropriate method of a command encoder.

See Simplifying GPU Resource Management with Residency Sets for more information.

## Topics

### Inspecting an Allocation

var allocatedSize: Int

The amount of memory, in byes, a resource consumes, such as for a buffer, texture, or heap.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTLAccelerationStructure
- MTLBuffer
- MTLHeap
- MTLIndirectCommandBuffer
- MTLIntersectionFunctionTable
- MTLResource
- MTLTexture
- MTLVisibleFunctionTable

## See Also

### Common Resource Functionality

protocol MTLResource

An allocation of memory accessible to a GPU.

struct MTLResourceOptions

Optional arguments used to set the behavior of a resource.

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

struct MTLResourceID

