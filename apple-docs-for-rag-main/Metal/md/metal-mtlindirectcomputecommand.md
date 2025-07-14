

- Metal
-  MTLIndirectComputeCommand 

Protocol

# MTLIndirectComputeCommand

A compute command in an indirect command buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
protocol MTLIndirectComputeCommand : NSObjectProtocol
```

## Overview

Don’t implement this protocol; you get objects of this type by asking a MTLIndirectCommandBuffer for them.

Use this object to reset or encode a command. You must always reset a command before encoding a new command.

## Topics

### Setting a Command’s Arguments

func setComputePipelineState(any MTLComputePipelineState)

Sets the command’s compute pipeline state object.

**Required**

func setImageblockWidth(Int, height: Int)

Sets the size, in pixels, of the imageblock.

**Required**

func setKernelBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a buffer for the compute function.

**Required**

func setThreadgroupMemoryLength(Int, index: Int)

Sets the size of a block of threadgroup memory.

**Required**

func setThreadgroupMemoryLength(Int, at: Int)

Sets the size of a block of threadgroup memory.

func setStageInRegion(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

**Required**

func setStageIn(MTLRegion)

Sets the region of the stage-in attributes to apply to the compute kernel.

### Synchronizing Command Execution

func setBarrier()

Adds a barrier to ensure that commands executed prior to this command are complete before this command executes.

**Required**

func clearBarrier()

Removes any barrier set on the command.

**Required**

### Encoding a Compute Command

func concurrentDispatchThreadgroups(MTLSize, threadsPerThreadgroup: MTLSize)

Encodes a compute command using a grid aligned to threadgroup boundaries.

**Required**

func concurrentDispatchThreads(MTLSize, threadsPerThreadgroup: MTLSize)

Encodes a compute command using an arbitrarily sized grid.

**Required**

### Resetting a Command

func reset()

Resets the command to its default state.

**Required**

### Instance Methods

func setKernelBuffer(any MTLBuffer, offset: Int, attributeStride: Int, at: Int)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Indirect Compute Commands

struct MTLRegion

The bounds for a subset of an object’s elements.

struct MTLSize

The dimensions of an object.

struct MTLOrigin

The coordinates for the front upper-left corner of a region.

struct MTLStageInRegionIndirectArguments

The data layout required for the arguments needed to specify the stage-in region.

struct MTLDispatchThreadgroupsIndirectArguments

The data layout required for arguments needed to specify the size of threadgroups.

