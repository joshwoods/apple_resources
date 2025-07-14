

- Metal
-  MTLCommandQueueDescriptor 

Class

# MTLCommandQueueDescriptor

A configuration that customizes the behavior for a new command queue.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class MTLCommandQueueDescriptor
```

## Topics

### Instance Properties

var logState: (any MTLLogState)?

The shader logging configuration that the command queue uses.

var maxCommandBufferCount: Int

An integer that sets the maximum number of uncompleted command buffers the queue can allow.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Submitting Work to a GPU

Setting Up a Command Structure

Discover how Metal executes commands on a GPU.

protocol MTLCommandQueue

An instance you use to create, submit, and schedule command buffers to a specific GPU device to run the commands within those buffers.

protocol MTLCommandBuffer

A container that stores a sequence of GPU commands that you encode into it.

class MTLCommandBufferDescriptor

A configuration that customizes the behavior for a new command buffer.

struct MTLCommandBufferError

The command buffer error codes that indicate why the GPU doesn’t finish executing a command buffer.

protocol MTLCommandEncoder

An encoder that writes GPU commands into a command buffer.

