

- Metal
- MTLIOCommandQueueDescriptor
-  maxCommandsInFlight 

Instance Property

# maxCommandsInFlight

Sets the largest number of individual commands that an input/output command queue can run at a time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var maxCommandsInFlight: Int { get set }
```

## Discussion

Set to `0` to instruct Metal to select an appropriate value for you — based on the system’s available memory.

## See Also

### Configuring the Input/Output Command Queue

var priority: MTLIOPriority

Configures the priority for a new input/output command queue.

var type: MTLIOCommandQueueType

Configures the queue type for a new input/output command queue.

var maxCommandBufferCount: Int

Sets the largest number of outstanding input/output command buffers a queue can have at any point in time.

