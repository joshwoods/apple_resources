

- Metal
-  MTLIOScratchBuffer 

Protocol

# MTLIOScratchBuffer

A protocol your app implements that wraps a Metal buffer instance to serve as scratch memory for an input/output command queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLIOScratchBuffer : NSObjectProtocol
```

## Overview

Your app can reintegrate a MTLIOScratchBuffer instance’s underlying memory back into a memory pool by overriding your type’s dealloc method. The system calls the method when an input/output command queue no longer needs a scratch buffer.

## Topics

### Wrapping a Buffer

var buffer: any MTLBuffer

A Metal buffer that serves as scratch memory for an input/output command queue.

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

protocol MTLIOScratchBufferAllocator

A protocol your app implements to provide scratch memory to an input/output command queue.

