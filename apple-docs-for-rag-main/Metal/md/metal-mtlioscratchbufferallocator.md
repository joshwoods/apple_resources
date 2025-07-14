

- Metal
-  MTLIOScratchBufferAllocator 

Protocol

# MTLIOScratchBufferAllocator

A protocol your app implements to provide scratch memory to an input/output command queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLIOScratchBufferAllocator : NSObjectProtocol
```

## Overview

An allocator returns instances of MTLIOScratchBuffer, another type your app implements.

## Topics

### Providing Scratch Memory to a Queue

func makeScratchBuffer(minimumSize: Int) -> (any MTLIOScratchBuffer)?

Creates a scratch memory buffer for an input/output command queue.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### I/O Command Queues

protocol MTLIOCommandQueue

A command queue that schedules input/output commands for reading files in the file system, and writing to GPU resources and memory.

class MTLIOCommandQueueDescriptor

A configuration template you use to create a new input/output command queue.

enum MTLIOPriority

Designates the priority for a new input/output command queue.

enum MTLIOCommandQueueType

Designates the queue type for a new input/output command queue.

protocol MTLIOScratchBuffer

A protocol your app implements that wraps a Metal buffer instance to serve as scratch memory for an input/output command queue.

