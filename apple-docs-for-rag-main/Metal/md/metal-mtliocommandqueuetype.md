

- Metal
-  MTLIOCommandQueueType 

Enumeration

# MTLIOCommandQueueType

Designates the queue type for a new input/output command queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLIOCommandQueueType
```

## Topics

### I/O Command Queue Types

case concurrent

Sets a new input/output command queue’s type to a queue that runs commands concurrently.

case serial

Sets a new input/output command queue’s type to a queue that runs commands serially.

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

### I/O Command Queues

protocol MTLIOCommandQueue

A command queue that schedules input/output commands for reading files in the file system, and writing to GPU resources and memory.

class MTLIOCommandQueueDescriptor

A configuration template you use to create a new input/output command queue.

enum MTLIOPriority

Designates the priority for a new input/output command queue.

protocol MTLIOScratchBufferAllocator

A protocol your app implements to provide scratch memory to an input/output command queue.

protocol MTLIOScratchBuffer

A protocol your app implements that wraps a Metal buffer instance to serve as scratch memory for an input/output command queue.

