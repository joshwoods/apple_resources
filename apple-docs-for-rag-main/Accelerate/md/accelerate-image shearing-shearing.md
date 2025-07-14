

- Accelerate
-  Image shearing 

API Collection

# Image shearing

Shear images horizontally and vertically.

## Topics

### Shearing an image horizontally

Single-precision horizontal shearing

Apply single-precision horizontal shearing to images.

Double-precision horizontal shearing

Apply double-precision horizontal shearing to images.

### Shearing an image vertically

Single-precision vertical shearing

Apply single-precision vertical shearing to images.

Double-precision vertical shearing

Apply double-precision vertical shearing to images.

### Resampling filters

func vImageNewResamplingFilter(Float, vImage_Flags) -> ResamplingFilter!

Creates a resampling filter object that corresponds to the default kernel supplied by the vImage framework.

func vImageNewResamplingFilterForFunctionUsingBuffer(ResamplingFilter, Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Creates a resampling filter object that encapsulates a resampling kernel function that you provide.

func vImageGetResamplingFilterExtent(ResamplingFilter, vImage_Flags) -> vImagePixelCount

Returns the maximum sampling radius for a resampling filter.

func vImageGetResamplingFilterSize(Float, ((UnsafePointer&lt;Float>?, UnsafeMutablePointer&lt;Float>?, UInt, UnsafeMutableRawPointer?) -> Void)!, Float, vImage_Flags) -> Int

Returns the minimum size, in bytes, for the buffer needed by the new resampling filter function.

func vImageDestroyResamplingFilter(ResamplingFilter!)

Disposes of a resampling filter object.

## See Also

### Image Resampling

Resampling in vImage

Learn how vImage resamples image data during geometric operations.

Reducing artifacts with custom resampling filters

Implement custom linear interpolation to prevent the ringing effects associated with scaling an image with the default Lanczos algorithm.

