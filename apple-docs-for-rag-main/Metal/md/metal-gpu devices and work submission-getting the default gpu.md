

- Metal
- GPU Devices and Work Submission
-  Getting the Default GPU 

Article

# Getting the Default GPU

Select the system’s default GPU device on which to run your Metal code.

## Overview

To use the Metal framework, start by getting a GPU device. All of the objects your app needs to interact with Metal come from a MTLDevice that you acquire at runtime. Some devices, such as those with iOS and tvOS have a single GPU that you can access by calling MTLCreateSystemDefaultDevice().

```
if(!(device = MTLCreateSystemDefaultDevice()))
{
    NSLog(@"Failed to get the system's default Metal device.");
}
```

On macOS devices that have multiple GPUs, such as a MacBook Pro, the system default is the discrete GPU.

## See Also

### Locating and Inspecting a GPU Device

Detecting GPU Features and Metal Software Versions

Use the device object’s properties to determine how you perform tasks in Metal.

func MTLCreateSystemDefaultDevice() -> (any MTLDevice)?

Returns the device instance Metal selects as the default.

protocol MTLDevice

The main Metal interface to a GPU that apps use to draw graphics and run computations in parallel.

Multi-GPU Systems

Locate and work with internal and external GPUs and their displays, video memory, and performance tradeoffs.

