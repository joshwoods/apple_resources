

- Metal
-  MTLCreateSystemDefaultDevice() 

Function

# MTLCreateSystemDefaultDevice()

Returns the device instance Metal selects as the default.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func MTLCreateSystemDefaultDevice() -> (any MTLDevice)?
```

## Return Value

A device object.

## Mentioned in 

Developing Metal apps that run in Simulator

Getting the Default GPU

## Discussion

In macOS, in order for the system to provide a default Metal device object, you must link to the Core Graphics framework. You usually need to do this explicitly if you’re writing apps that don’t use graphics by default, such as command line tools.

## See Also

### Locating and Inspecting a GPU Device

Getting the Default GPU

Select the system’s default GPU device on which to run your Metal code.

Detecting GPU Features and Metal Software Versions

Use the device object’s properties to determine how you perform tasks in Metal.

protocol MTLDevice

The main Metal interface to a GPU that apps use to draw graphics and run computations in parallel.

Multi-GPU Systems

Locate and work with internal and external GPUs and their displays, video memory, and performance tradeoffs.

