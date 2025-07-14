

- Accelerate
-  vImagePerspectiveWarp_ARGB8888(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImagePerspectiveWarp_ARGB8888(\_:\_:\_:\_:\_:\_:\_:)

Applies a perspective warp to an 8-bit-per-channel, four-channel interleaved image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func vImagePerspectiveWarp_ARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ transform: UnsafePointer,
    _ interpolation: vImage_WarpInterpolation,
    _ backColor: UnsafeMutablePointer!,
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

`transform`  

The vImage_PerpsectiveTransform structure that the operation applies to the source buffer.

`interpolation`  

The `vImage_WarpInterpolation` enumeration that specifies the interpolation mode.

`backColor`  

The background color. If you set the kvImageBackgroundColorFill flag, pass a pixel value.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

To specify how vImage handles pixel locations beyond the edge of the source image, set one of the following flags: kvImageBackgroundColorFill or kvImageEdgeExtend.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Mentioned in 

Transforming an image in three dimensions

## Discussion

This function doesn’t work in place, that is, the source and destination buffers must point to different underlying memory.

## See Also

### Related Documentation

Transforming an image in three dimensions

Create and use a projective transformation to apply a perspective warp to an image.

### Warping interleaved buffers

func vImagePerspectiveWarp_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, UnsafeMutablePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a perspective warp to a floating-point 16-bit , four-channel interleaved image.

func vImagePerspectiveWarp_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, UnsafeMutablePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a perspective warp to an unsigned 16-bit , four-channel interleaved image.

