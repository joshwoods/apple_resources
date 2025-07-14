

- Accelerate
-  vImageAffineWarpD_Planar8(\_:\_:\_:\_:\_:\_:) 

Function

# vImageAffineWarpD_Planar8(\_:\_:\_:\_:\_:\_:)

Applies a double-precision affine transformation to an 8-bit planar image.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 6.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageAffineWarpD_Planar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ transform: UnsafePointer,
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

`transform`  

The affine transformation matrix that the function applies to the source image.

`backColor`  

A background color. If you set the `kvImageBackgroundColorFill` flag, pass a pixel value.

`flags`  

The options to use when applying the transform.

To specify how vImage handles pixel locations beyond the edge of the source image, set one of the following flags: kvImageBackgroundColorFill or kvImageEdgeExtend.

If you want vImage to use a higher quality but a slower resampling filter, set the kvImageHighQualityResampling flag.

If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

This function ignores the kvImageLeaveAlphaUnchanged flag.

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

This function maps each pixel in the source image `[x, y]` to a new position `[x’, y’]` in the destination image using the following formula:

```
(x', y') = (x, y) * transform
```

In the preceding function, `transform` is the 3 x 3 affine transformation matrix.

The coordinate space places the origin at the bottom-left corner of the image. Positive movement in the horizontal direction moves pixels to the right. Positive movement in the vertical direction moves pixels up.

To avoid artifacts in high-frequency regions of the image, supply image data that’s nonpremultiplied or that has a constant alpha over the entire image.

This function doesn’t work in place — that is, the source and destination buffers must point to different memory.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Double-Precision Affine Transformation

func vImageAffineWarpD_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, Pixel_F, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a 32-bit planar image.

func vImageAffineWarpD_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, Pixel_16F, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a floating-point 16-bit planar image.

func vImageAffineWarpD_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a floating-point 16-bit-per-channel, 2-channel interleaved image.

func vImageAffineWarpD_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to an 8-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to an unsigned 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a signed 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a floating-point 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a 32-bit-per-channel, 4-channel interleaved image.

