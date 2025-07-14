

- Metal
- MTLCommandBuffer
-  gpuEndTime 

Instance Property

# gpuEndTime

The host time, in seconds, when the GPU finishes execution of the command buffer.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.0+macOS 10.15+tvOS 10.2+visionOS 1.0+

``` source
var gpuEndTime: CFTimeInterval { get }
```

**Required**

## Discussion

You can calculate how much time the GPU spends running a command buffer by subtracting gpuStartTime from this value. Both values are relative to system mach time.

The GPU start and end times remain `0.0` until the GPU finishes running the command buffer. Check this value after the waitUntilCompleted() method returns, or within a completion handler passed to the addCompletedHandler(_:) method.

## See Also

### Checking Execution Times on the GPU

var gpuStartTime: CFTimeInterval

The host time, in seconds, when the GPU starts command buffer execution.

**Required**

