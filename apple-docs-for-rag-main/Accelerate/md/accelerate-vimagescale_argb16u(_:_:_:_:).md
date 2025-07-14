

- Accelerate
-  vImageScale_ARGB16U(\_:\_:\_:\_:) 

Function

# vImageScale_ARGB16U(\_:\_:\_:\_:)

Scales an unsigned 16-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageScale_ARGB16U(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to a vImage buffer structure that contains the source image.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `nil`, the function allocates the buffer and then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you’re responsible for deallocating it when you no longer need it.

`flags`  

The options to use when applying the scale.

If you want vImage to use a higher quality but a slower resampling filter, set the kvImageHighQualityResampling flag.

If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

This function ignores the kvImageLeaveAlphaUnchanged flag.

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

The relative dimensions of the source image and the destination buffer determine the scaling factors. The function supports nonuniform scaling — that is, the horizontal and vertical ratios can be different.

To avoid artifacts in high-frequency regions of the image, supply image data that’s nonpremultiplied or that has a constant alpha over the entire image.

This function doesn’t work in place — that is, the source and destination buffers must point to different memory.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Interleaved Image Scaling

func vImageScale_CbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an 8-bit-per-channel, 2-channel interleaved image to fit a destination buffer.

func vImageScale_CbCr16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an unsigned 16-bit-per-channel, 2-channel interleaved image to fit a destination buffer.

func vImageScale_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a floating-point 16-bit-per-channel, 2-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an 8-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a signed 16-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a floating-point 16-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a 32-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_XRGB2101010W(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a 2-bit alpha, 10-bit RGB interleaved image to fit a destination buffer.

