

- Metal
- MTLCommandBuffer
-  status 

Instance Property

# status

The command buffer’s current state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var status: MTLCommandBufferStatus { get }
```

**Required**

## Mentioned in 

Setting Up a Command Structure

Preparing Your Metal App to Run in the Background

## Discussion

Each command buffer can be in any one of the following states:

| State | Meaning |
|----|----|
| MTLCommandBufferStatus.notEnqueued | A command buffer’s initial state, which indicates its command queue isn’t reserving a place for it.  You can modify a command buffer in this state by encoding commands to it, or by adding a state change handler. |
| MTLCommandBufferStatus.enqueued | A command buffer’s second state, which indicates its command queue is reserving a place for it.  You can modify a command buffer in this state by encoding commands to it, or by adding a state change handler. |
| MTLCommandBufferStatus.committed | A command buffer’s third state, which indicates the command queue is preparing to schedule the command buffer by resolving its dependencies.  You can’t modify a command buffer in this state. |
| MTLCommandBufferStatus.scheduled | A command buffer’s fourth state, which indicates the command buffer has its resources ready and is waiting for the GPU to run its commands.  You can’t modify a command buffer in this state. |
| MTLCommandBufferStatus.completed | A command buffer’s successful, final state, which indicates the GPU finished running the command buffer’s commands without any problems. |
| MTLCommandBufferStatus.error | A command buffer’s unsuccessful, final state, which indicates the GPU stopped running the buffer’s commands because of a runtime issue. |

The first two states (MTLCommandBufferStatus.notEnqueued and MTLCommandBufferStatus.enqueued) both indicate that you can encode commands to the command buffer. You do this by creating an encoder that indirectly adds commands for a pass (see Command Encoder Factory Methods) to the command buffer. Command buffers also have some methods that directly encode commands between passes, such as encodeSignalEvent(_:value:) and present(_:).

Each command buffer’s state can only change to a state below it in the table, and ends its life cycle at either MTLCommandBufferStatus.completed or MTLCommandBufferStatus.error.

## See Also

### Troubleshooting a Command Buffer

enum MTLCommandBufferStatus

The discrete states for a command buffer that represent its life cycle stages.

Command Buffer Debugging

Properties and methods for programmatically debugging runtime issues with a command buffer.

