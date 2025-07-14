

- Metal
- MTLCommandBuffer
-  waitUntilScheduled() 

Instance Method

# waitUntilScheduled()

Blocks the current thread until the command queue schedules the buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func waitUntilScheduled()
```

**Required**

## Mentioned in 

Preparing Your Metal App to Run in the Background

## Discussion

This method returns after the following events:

- The command queue *schedules* (see status and MTLCommandBufferStatus.scheduled) the command buffer to run on the GPU.

- The command buffer invokes all the completion handlers your app submits with addScheduledHandler(_:).

Use the waitUntilCompleted() method to check for completion of the scheduled work.

## See Also

### Waiting for State Changes

func waitUntilCompleted()

Blocks the current thread until the GPU finishes executing the command buffer and all of its completion handlers.

**Required**

