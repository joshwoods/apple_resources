

- Metal
- MTLIOCommandQueueDescriptor
-  priority 

Instance Property

# priority

Configures the priority for a new input/output command queue.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var priority: MTLIOPriority { get set }
```

## See Also

### Configuring the Input/Output Command Queue

var type: MTLIOCommandQueueType

Configures the queue type for a new input/output command queue.

var maxCommandsInFlight: Int

Sets the largest number of individual commands that an input/output command queue can run at a time.

var maxCommandBufferCount: Int

Sets the largest number of outstanding input/output command buffers a queue can have at any point in time.

