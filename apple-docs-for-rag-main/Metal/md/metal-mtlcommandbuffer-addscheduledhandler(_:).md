

- Metal
- MTLCommandBuffer
-  addScheduledHandler(\_:) 

Instance Method

# addScheduledHandler(\_:)

Registers a completion handler the GPU device calls immediately after it schedules the command buffer to run on the GPU.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func addScheduledHandler(_ block: @escaping MTLCommandBufferHandler)
```

**Required**

## Parameters 

`block`  

A Swift closure or an Objective-C block that Metal calls after it schedules the command buffer to run on the GPU.

## Mentioned in 

Setting Up a Command Structure

## Discussion

You can register one or more scheduling completion handlers for the same command buffer. The GPU device’s driver (on the CPU) calls the completion handlers after it finishes scheduling the command buffer to run on the GPU.

Important

You can only call this method before calling the command buffer’s commit() method.

The GPU device schedules each command buffer — along with tasks from other command buffers — after it identifies the command buffer’s dependencies. At that time, the GPU device sets the command buffer’s status to MTLCommandBufferStatus.scheduled and calls your completion handler.

Note

The command buffer’s status property may be equal to another (larger) value by the time your completion handler runs, including MTLCommandBufferStatus.completed.

You can use the command buffer’s kernelEndTime and kernelStartTime properties to calculate how much time the CPU spends scheduling the command buffer.

- Swift
- Objective-C

```
commandBuffer.addScheduledHandler { commandBuffer in
    let start = commandBuffer.kernelStartTime
    let end = commandBuffer.kernelEndTime

    let scheduleDuration = end - start

    /* ... */
}
```

```
[commandBuffer addScheduledHandler:^(id commandBuffer) {
    CFTimeInterval start = commandBuffer.kernelStartTime;
    CFTimeInterval end = commandBuffer.kernelEndTime;

    CFTimeInterval scheduleDuration = end - start;

    /* ... */
}];

```

## See Also

### Registering State Change Handlers

func addCompletedHandler(MTLCommandBufferHandler)

Registers a completion handler the GPU device calls immediately after the GPU finishes running the commands in the command buffer.

**Required**

typealias MTLCommandBufferHandler

A completion handler signature a GPU device calls when it finishes scheduling a command buffer, or when the GPU finishes running it.

