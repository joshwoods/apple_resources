

- Metal
-  MTLIOCommandQueue 

Protocol

# MTLIOCommandQueue

A command queue that schedules input/output commands for reading files in the file system, and writing to GPU resources and memory.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLIOCommandQueue : NSObjectProtocol
```

## Overview

Use an input/output command queue to submit commands, in command buffers, that load assets from the file system directly into GPU resources. Your app can then use those resources with other commands it submits to an MTLCommandQueue that comes from the same MTLDevice.

You make input/output command queues by creating and configuring an MTLIOCommandQueueDescriptor instance and calling an MTLDevice instance’s makeIOCommandQueue(descriptor:) method.

## Topics

### Creating a Input/Output Command Buffer

func makeCommandBuffer() -> any MTLIOCommandBuffer

Creates an input/output command buffer for the command queue.

**Required**

func makeCommandBufferWithUnretainedReferences() -> any MTLIOCommandBuffer

Creates an input/output command buffer for the command queue that doesn’t retain the instances you pass to its methods.

**Required**

### Adding a Barrier to the Queue

func enqueueBarrier()

Appends a barrier that tells the input/output command queue to finish running all in-flight command buffers before running any new command buffers.

**Required**

### Naming the Queue

var label: String?

An optional name for the input/output command queue.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### I/O Command Queues

class MTLIOCommandQueueDescriptor

A configuration template you use to create a new input/output command queue.

enum MTLIOPriority

Designates the priority for a new input/output command queue.

enum MTLIOCommandQueueType

Designates the queue type for a new input/output command queue.

protocol MTLIOScratchBufferAllocator

A protocol your app implements to provide scratch memory to an input/output command queue.

protocol MTLIOScratchBuffer

A protocol your app implements that wraps a Metal buffer instance to serve as scratch memory for an input/output command queue.

