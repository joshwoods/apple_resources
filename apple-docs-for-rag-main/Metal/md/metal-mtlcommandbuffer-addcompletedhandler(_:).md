

- Metal
- MTLCommandBuffer
-  addCompletedHandler(\_:) 

Instance Method

# addCompletedHandler(\_:)

Registers a completion handler the GPU device calls immediately after the GPU finishes running the commands in the command buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func addCompletedHandler(_ block: @escaping MTLCommandBufferHandler)
```

**Required**

## Parameters 

`block`  

A Swift closure or an Objective-C block that Metal calls after the GPU finishes running the commands in the command buffer.

## Mentioned in 

Setting Up a Command Structure

Converting a GPU’s Counter Data into a Readable Format

Preparing Your Metal App to Run in the Background

## Discussion

You can register one or more completion handlers for the same command buffer. The GPU device’s driver (on the CPU) calls the completion handlers after the GPU finishes executing the command buffer.

Important

You can only call this method before calling the command buffer’s commit() method.

For example, you can use the command buffer’s gpuEndTime and gpuStartTime properties to calculate how much time the GPU spends running the command buffer.

- Swift
- Objective-C

```
commandBuffer.addCompletedHandler { commandBuffer in
    let start = commandBuffer.gpuStartTime
    let end = commandBuffer.gpuEndTime

    let gpuRuntimeDuration = end - start

    /* ... */
}
```

```
[commandBuffer addCompletedHandler:^(id commandBuffer) {
    CFTimeInterval start = commandBuffer.GPUStartTime;
    CFTimeInterval end = commandBuffer.GPUEndTime;

    CFTimeInterval gpuRuntimeDuration = end - start;

    /* ... */
}];
```

The completion handler is also a good place to check the status property to determine whether the GPU successfully completes the buffer’s commands. If the status is equal to MTLCommandBufferStatus.error, you can investigate further by checking the error and log properties for more details about the issue. See Command Buffer Debugging for more methods and properties that can help you isolate the issue.

Warning

Avoid calling the insertDebugCaptureBoundary() method within the completion handler, which can cause a debug-time deadlock if you request GPU frame capture.

## See Also

### Registering State Change Handlers

func addScheduledHandler(MTLCommandBufferHandler)

Registers a completion handler the GPU device calls immediately after it schedules the command buffer to run on the GPU.

**Required**

typealias MTLCommandBufferHandler

A completion handler signature a GPU device calls when it finishes scheduling a command buffer, or when the GPU finishes running it.

