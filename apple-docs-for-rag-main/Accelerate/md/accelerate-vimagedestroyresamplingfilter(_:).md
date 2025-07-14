

- Accelerate
-  vImageDestroyResamplingFilter(\_:) 

Function

# vImageDestroyResamplingFilter(\_:)

Disposes of a resampling filter object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageDestroyResamplingFilter(_ filter: ResamplingFilter!)
```

## Parameters 

`filter`  

The resampling filter object to dispose of.

## Discussion

This function deallocates the memory associated with a resampling filter object that was created by calling the function vImageNewResamplingFilter(_:_:). Don’t directly deallocate this memory yourself.

Don’t pass this function a resampling filter object created by the function vImageNewResamplingFilterForFunctionUsingBuffer(_:_:_:_:_:_:). You’re responsible for deallocating the memory associated with resampling filter objects created by that call.

## See Also

### Resampling filters

func vImageNewResamplingFilter(Float, vImage_Flags) -> ResamplingFilter!

Creates a resampling filter object that corresponds to the default kernel supplied by the vImage framework.

func vImageNewResamplingFilterForFunctionUsingBuffer(ResamplingFilter, Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Creates a resampling filter object that encapsulates a resampling kernel function that you provide.

func vImageGetResamplingFilterExtent(ResamplingFilter, vImage_Flags) -> vImagePixelCount

Returns the maximum sampling radius for a resampling filter.

func vImageGetResamplingFilterSize(Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, vImage_Flags) -> Int

Returns the minimum size, in bytes, for the buffer needed by the new resampling filter function.

