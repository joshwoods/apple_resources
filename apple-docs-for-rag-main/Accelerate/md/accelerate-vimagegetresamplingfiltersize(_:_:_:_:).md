

- Accelerate
-  vImageGetResamplingFilterSize(\_:\_:\_:\_:) 

Function

# vImageGetResamplingFilterSize(\_:\_:\_:\_:)

Returns the minimum size, in bytes, for the buffer needed by the new resampling filter function.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageGetResamplingFilterSize(
    _ scale: Float,
    _ kernelFunc: ((UnsafePointer?, UnsafeMutablePointer?, UInt, UnsafeMutableRawPointer?) -> Void)!,
    _ kernelWidth: Float,
    _ flags: vImage_Flags
) -> Int
```

## Parameters 

`scale`  

The scale factor that you plan to pass to the function `vImageNewResamplingFilterForFunctionUsingBuffer`.

`kernelFunc`  

The function pointer that you plan to pass to the function `vImageNewResamplingFilterForFunctionUsingBuffer`.

`kernelWidth`  

The kernel width that you plan to pass to the function `vImageNewResamplingFilterForFunctionUsingBuffer`.

`flags`  

The flags that you plan to pass to the function `vImageNewResamplingFilterForFunctionUsingBuffer`.

## Return Value

The minimum size, in bytes, of the buffer.

## See Also

### Resampling filters

func vImageNewResamplingFilter(Float, vImage_Flags) -> ResamplingFilter!

Creates a resampling filter object that corresponds to the default kernel supplied by the vImage framework.

func vImageNewResamplingFilterForFunctionUsingBuffer(ResamplingFilter, Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Creates a resampling filter object that encapsulates a resampling kernel function that you provide.

func vImageGetResamplingFilterExtent(ResamplingFilter, vImage_Flags) -> vImagePixelCount

Returns the maximum sampling radius for a resampling filter.

func vImageDestroyResamplingFilter(ResamplingFilter!)

Disposes of a resampling filter object.

