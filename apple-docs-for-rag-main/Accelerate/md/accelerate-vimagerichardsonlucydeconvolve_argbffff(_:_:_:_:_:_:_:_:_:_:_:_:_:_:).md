

- Accelerate
-  vImageRichardsonLucyDeConvolve_ARGBFFFF(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageRichardsonLucyDeConvolve_ARGBFFFF(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Deconvolves a floating-point 32-bit-per-channel, 4-channel interleaved image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageRichardsonLucyDeConvolve_ARGBFFFF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ srcOffsetToROI_X: vImagePixelCount,
    _ srcOffsetToROI_Y: vImagePixelCount,
    _ kernel: UnsafePointer!,
    _ kernel2: UnsafePointer!,
    _ kernel_height: UInt32,
    _ kernel_width: UInt32,
    _ kernel_height2: UInt32,
    _ kernel_width2: UInt32,
    _ backgroundColor: UnsafePointer!,
    _ iterationCount: UInt32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to a vImage buffer structure that contains data for the source image.

`dest`  

A pointer to a vImage buffer data structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, you must deallocate the memory.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `NULL`, the function allocates the buffer, then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you are responsible for deallocating it when you is no longer need it.

If you want to allocate the buffer yourself, see the Discussion for information on how to determine the minimum size that you must allocate.

`srcOffsetToROI_X`  

The horizontal offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`srcOffsetToROI_Y`  

The vertical offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`kernel`  

A pointer to the deconvolution kernel data, which must be a packed array without any padding. The kernel expresses a blurring convolution or point-spread function.

`kernel2`  

A pointer to the data of a second kernel, which must be a packed array without any padding. Supply this kernel only if the first kernel is asymmetrical; otherwise pass `NULL`.

`kernel_height`  

The height of the first kernel in pixels. This value must be odd.

`kernel_width`  

The width of the first kernel in pixels. This value must be odd.

`kernel_height2`  

The height of the second kernel in pixels (ignored if `kernel2` is `NULL`). This value must be odd.

`kernel_width2`  

The width of the second kernel in pixels (ignored if `kernel2` is `NULL`). This value must be odd.

`backgroundColor`  

A background color. If you supply a color, you must also set the `kvImageBackgroundColorFill` flag, otherwise the function ignores the color.

`iterationCount`  

The number of times to iterate the deconvolution algorithm.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

Pass one of the following flags to specify how vImage handles pixel locations beyond the edge of the source image: kvImageCopyInPlace, kvImageTruncateKernel, kvImageBackgroundColorFill, or kvImageEdgeExtend.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function performs a Richardson-Lucy deconvolution of a region of interest within a source image by an M x N kernel, performing a specified number of iterations and placing the result in a destination buffer.

If you want to allocate the memory for the `tempBuffer` parameter yourself, call this function twice, as follows:

1.  To determine the minimum size for the temporary buffer, the first time you call this function pass the `kvImageGetTempBufferSize` flag. Pass the same values for all other parameters that you intend to use in for the second call. The function returns the required minimum size, which should be a positive value. (A negative returned value indicates an error.) The `kvImageGetTempBufferSize` flag prevents the function from performing any processing other than to determine the minimum buffer size.

2.  After you allocate enough space for a buffer of the returned size, call the function a second time, passing a valid pointer in the `tempBuffer` parameter. This time, do not pass the `kvImageGetTempBufferSize` flag.

## See Also

### Related Documentation

vImage Programming Guide

### Deconvolving

func vImageRichardsonLucyDeConvolve_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Int16>!, UnsafePointer&lt;Int16>!, UInt32, UInt32, UInt32, UInt32, Int32, Int32, Pixel_8, UInt32, vImage_Flags) -> vImage_Error

Deconvolves an 8-bit planar image.

func vImageRichardsonLucyDeConvolve_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, UInt32, UInt32, UInt32, UInt32, Pixel_F, UInt32, vImage_Flags) -> vImage_Error

Deconvolves a floating-point 32-bit planar image.

func vImageRichardsonLucyDeConvolve_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Int16>!, UnsafePointer&lt;Int16>!, UInt32, UInt32, UInt32, UInt32, Int32, Int32, UnsafePointer&lt;UInt8>!, UInt32, vImage_Flags) -> vImage_Error

Deconvolves an 8-bit-per-channel, 4-channel interleaved image.

