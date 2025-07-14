

- Accelerate
-  vImageAffineWarpCG_PlanarF(\_:\_:\_:\_:\_:\_:) 

Function

# vImageAffineWarpCG_PlanarF(\_:\_:\_:\_:\_:\_:)

Applies a Core Graphics affine transformation to a PlanarF source image.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 6.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageAffineWarpCG_PlanarF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ transform: UnsafePointer,
    _ backColor: Pixel_F,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to a vImage buffer structure that contains the source image whose data you want to transform.

`dest`  

A pointer to a vImage buffer data structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, you must deallocate the memory.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `NULL`, the function allocates the buffer, then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you’re responsible for deallocating it when you no longer need it.

If you want to allocate the buffer yourself, see Allocating Temporary Buffer Memory for information on how to determine the minimum size that you must allocate.

`transform`  

The affine transformation matrix to apply to the source image.

`backColor`  

A background color. Pass a pixel value only if you also set the `kvImageBackgroundColorFill` flag.

`flags`  

The options to use when applying the rotation.

To specify how vImage handles pixel locations beyond the edge of the source image, you must set exactly one of the following flags: kvImageBackgroundColorFill or kvImageEdgeExtend.

If you want vImage to use a higher quality, but slower resampling filter, set the kvImageHighQualityResampling flag.

If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

This function ignores the kvImageLeaveAlphaUnchanged flag.

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

Core Graphics types use float values in 32-bit and double values in 64-bit. This convenience method takes the Core Graphics affine transform type directly so that you don’t have to use a different function for 64-bit applications.

This function maps each pixel in the source image `[x, y]` to a new position `[x’, y’]` in the destination image, using this formula:

```
(x', y') = (x, y) * transform
```

where `transform` is the 3x3 affine transformation matrix.

### Allocating Temporary Buffer Memory

If you want to allocate the memory for the `tempBuffer` parameter yourself, call this function twice, as follows:

1.  To determine the minimum size for the temporary buffer, the first time you call this function, pass the kvImageGetTempBufferSize flag. Pass the same values for all other parameters that you intend to use for the second call. The function returns the required minimum size, which should be a positive value. (A negative returned value indicates an error.) The `kvImageGetTempBufferSize` flag prevents the function from performing any processing other than to determine the minimum buffer size.

2.  After you allocate enough space for a buffer of the returned size, call the function a second time, passing a valid pointer in the `tempBuffer` parameter. This time, don’t pass the kvImageGetTempBufferSize flag.

## See Also

### Core Graphics Affine Transformation

func vImageAffineWarpCG_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, Pixel_8, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to a Planar8 source image.

func vImageAffineWarpCG_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGB16U source image.

func vImageAffineWarpCG_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGB16S source image.

func vImageAffineWarpCG_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGB8888 source image.

func vImageAffineWarpCG_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGBFFFF source image.

