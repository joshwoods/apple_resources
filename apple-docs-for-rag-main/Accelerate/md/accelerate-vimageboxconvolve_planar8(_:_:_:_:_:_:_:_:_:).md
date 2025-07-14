

- Accelerate
-  vImageBoxConvolve_Planar8(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageBoxConvolve_Planar8(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a box filter to an 8-bit planar source image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageBoxConvolve_Planar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ srcOffsetToROI_X: vImagePixelCount,
    _ srcOffsetToROI_Y: vImagePixelCount,
    _ kernel_height: UInt32,
    _ kernel_width: UInt32,
    _ backgroundColor: Pixel_8,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to a vImage buffer structure that contains data for the source image.

`dest`  

A pointer to a vImage buffer data structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, you must deallocate the memory. The size (number of rows and number of columns) of the destination buffer also specifies the size of the region of interest in the source buffer.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `NULL`, the function allocates the buffer, then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you are responsible for deallocating it when you is no longer need it.

If you want to allocate the buffer yourself, see the Discussion for information on how to determine the minimum size that you must allocate.

`srcOffsetToROI_X`  

The horizontal offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`srcOffsetToROI_Y`  

The vertical offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`kernel_height`  

The height of the kernel in pixels. This value must be odd.

`kernel_width`  

The width of the kernel in pixels. This value must be odd.

`backgroundColor`  

A background color. If you supply a color, you must also set the `kvImageBackgroundColorFill` flag, otherwise the function ignores the color.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

Pass one of the following flags to specify how vImage handles pixel locations beyond the edge of the source image: kvImageCopyInPlace, kvImageTruncateKernel, kvImageBackgroundColorFill, or kvImageEdgeExtend.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function uses an implicit divisor and an implicit kernel of specified size instead of a kernel provided by the caller.

If you want to allocate the memory for the `tempBuffer` parameter yourself, call this function twice, as follows:

1.  To determine the minimum size for the temporary buffer, the first time you call this function pass the `kvImageGetTempBufferSize` flag. Pass the same values for all other parameters that you intend to use in for the second call. The function returns the required minimum size, which should be a positive value. (A negative returned value indicates an error.) The `kvImageGetTempBufferSize` flag prevents the function from performing any processing other than to determine the minimum buffer size.

2.  After you allocate enough space for a buffer of the returned size, call the function a second time, passing a valid pointer in the `tempBuffer` parameter. This time, do not pass the `kvImageGetTempBufferSize` flag.

## See Also

### Related Documentation

func vImageConvolve_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Int16>!, UInt32, UInt32, Int32, Pixel_8, vImage_Flags) -> vImage_Error

Convolves an 8-bit planar image by a 2D kernel and divides the pixel values by a divisor.

### Convolving with high-speed box and tent filters

func vImageBoxConvolve_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UInt32, UInt32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a box filter to an 8-bit-per-channel, 4-channel interleaved source image.

func vImageTentConvolve_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UInt32, UInt32, Pixel_8, vImage_Flags) -> vImage_Error

Applies a tent filter to an 8-bit planar source image.

func vImageTentConvolve_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UInt32, UInt32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a tent filter to an 8-bit-per-channel, 4-channel interleaved source image.

