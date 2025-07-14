

- Accelerate
-  vImageNewResamplingFilter(\_:\_:) 

Function

# vImageNewResamplingFilter(\_:\_:)

Creates a resampling filter object that corresponds to the default kernel supplied by the vImage framework.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageNewResamplingFilter(
    _ scale: Float,
    _ flags: vImage_Flags
) -> ResamplingFilter!
```

## Parameters 

`scale`  

A scale factor to associated with the resampling filter object. Shear functions to which you pass the resampling filter object use this factor when performing a shear operation. The shear function applies the scale factor to the entire image, in a direction appropriate to the shear function, either horizontal or vertical.

`flags`  

The options to use when creating the resampling filter object. You must set exactly one of the following flags to specify how vImage handles pixel locations beyond the edge of the source image: kvImageBackgroundColorFill or kvImageEdgeExtend.

Set the kvImageHighQualityResampling flag if you want vImage to use a higher quality, but slower, resampling filter.

If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

This function ignores the kvImageLeaveAlphaUnchanged flag.

## Return Value

A pointer to a newly created resampling filter object; otherwise `NULL`.

## Discussion

This function creates a reusable resampling filter object that you can pass to a shear function. The resampling filter encapsulated by the object is the default kernel for vImage This function allocates the memory needed for the resampling filter object. To deallocate this memory, call the function vImageDestroyResamplingFilter(_:). Don’t attempt to deallocate the memory yourself.

## See Also

### Resampling filters

func vImageNewResamplingFilterForFunctionUsingBuffer(ResamplingFilter, Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Creates a resampling filter object that encapsulates a resampling kernel function that you provide.

func vImageGetResamplingFilterExtent(ResamplingFilter, vImage_Flags) -> vImagePixelCount

Returns the maximum sampling radius for a resampling filter.

func vImageGetResamplingFilterSize(Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, vImage_Flags) -> Int

Returns the minimum size, in bytes, for the buffer needed by the new resampling filter function.

func vImageDestroyResamplingFilter(ResamplingFilter!)

Disposes of a resampling filter object.

