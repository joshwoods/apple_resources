

- Metal
- MTLCommandBuffer
-  kernelEndTime 

Instance Property

# kernelEndTime

The host time, in seconds, when the CPU finishes scheduling the command buffer.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.0+macOS 10.15+tvOS 10.2+visionOS 1.0+

``` source
var kernelEndTime: CFTimeInterval { get }
```

**Required**

## Discussion

You can calculate how much time the kernel spends scheduling a command buffer by subtracting kernelStartTime from this value.

The kernel start and end times remain `0.0` until the GPU driver (on the CPU) schedules the command buffer to run on the GPU. Apps typically use these values after the waitUntilScheduled() method returns, or within a completion handler (see addScheduledHandler(_:) and addCompletedHandler(_:)).

## See Also

### Checking Scheduling Times on the CPU

var kernelStartTime: CFTimeInterval

The host time, in seconds, when the CPU begins to schedule the command buffer.

**Required**

