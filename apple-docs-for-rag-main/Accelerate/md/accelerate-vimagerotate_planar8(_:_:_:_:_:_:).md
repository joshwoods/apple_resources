

- Accelerate
-  vImageRotate_Planar8(\_:\_:\_:\_:\_:\_:) 

Function

# vImageRotate_Planar8(\_:\_:\_:\_:\_:\_:)

Rotates an 8-bit planar image by any angle, which you specify in radians.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageRotate_Planar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ angleInRadians: Float,
    _ backColor: Pixel_8,
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

`angleInRadians`  

The rotation angle, in radians.

`backColor`  

A background color. If you set the `kvImageBackgroundColorFill` flag, pass a pixel value.

`flags`  

The options to use when applying the rotation.

To specify how vImage handles pixel locations beyond the edge of the source image, set one of the following flags: kvImageBackgroundColorFill or kvImageEdgeExtend.

If you want vImage to use a higher quality but a slower resampling filter, set the kvImageHighQualityResampling flag.

If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

This function ignores the kvImageLeaveAlphaUnchanged flag.

## Return Value

kvImageNoError; otherwise, one of the error codes from Error codes.

## Discussion

This function maps the center point of the source image to the center point of the destination image. Depending on the relative sizes of the source image and the destination buffer, the function might clip parts of the source image. Areas outside the source image might appear in the destination image if you don’t pass a background color to the function.

To avoid artifacts in high-frequency regions of the image, supply image data that’s nonpremultiplied or that has a constant alpha over the entire image.

This function doesn’t work in place — that is, the source and destination buffers must point to different memory.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Rotating 8-bit-per-channel buffers by any angle

func vImageRotate_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Rotates an 8-bit-per-channel, 4-channel interleaved image by any angle, which you specify in radians.

