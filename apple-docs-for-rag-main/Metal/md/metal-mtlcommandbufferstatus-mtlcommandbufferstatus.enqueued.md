

- Metal
- MTLCommandBufferStatus
-  MTLCommandBufferStatus.enqueued 

Case

# MTLCommandBufferStatus.enqueued

A command buffer’s second state, which indicates its command queue is reserving a place for it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case enqueued
```

## Discussion

See the MTLCommandBuffer protocol’s status property for more information.

## See Also

### Command Buffer States

case notEnqueued

A command buffer’s initial state, which indicates its command queue isn’t reserving a place for it.

case committed

A command buffer’s third state, which indicates the command queue is preparing to schedule the command buffer by resolving its dependencies.

case scheduled

A command buffer’s fourth state, which indicates the command buffer has its resources ready and is waiting for the GPU to run its commands.

case completed

A command buffer’s successful, final state, which indicates the GPU finished running the command buffer’s commands without any problems.

case error

A command buffer’s unsuccessful, final state, which indicates the GPU stopped running the buffer’s commands because of a runtime issue.

