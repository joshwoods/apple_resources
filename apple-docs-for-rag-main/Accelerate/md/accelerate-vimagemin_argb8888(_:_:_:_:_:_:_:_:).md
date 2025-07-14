

- Accelerate
-  vImageMin_ARGB8888(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageMin_ARGB8888(\_:\_:\_:\_:\_:\_:\_:\_:)

Minimizes an 8-bit-per-channel, 4-channel interleaved buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageMin_ARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ srcOffsetToROI_X: vImagePixelCount,
    _ srcOffsetToROI_Y: vImagePixelCount,
    _ kernel_height: vImagePixelCount,
    _ kernel_width: vImagePixelCount,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `nil`, the function allocates the buffer and then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you’re responsible for deallocating it when you no longer need it.

`srcOffsetToROI_X`  

The horizontal offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`srcOffsetToROI_Y`  

The vertical offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`kernel_height`  

The height of the kernel in pixels. This value must be odd.

`kernel_width`  

The width of the kernel in pixels. This value must be odd.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

To specify that the function doesn’t apply the operation to the alpha channel, set the kvImageLeaveAlphaUnchanged flag.

To determine the minimum size for the temporary buffer, set the kvImageGetTempBufferSize flag.

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

The minimize filter is an optimized version of the erosion in which all the filter elements are zero.

### Allocating Temporary Buffer Memory

If you want to allocate the memory for the `tempBuffer` parameter yourself, call this function twice, as follows:

1.  To determine the minimum size for the temporary buffer, the first time you call this function, pass the kvImageGetTempBufferSize flag. Pass the same values for all other parameters that you intend to use for the second call. The function returns the required minimum size, which should be a positive value (a negative returned value indicates an error). The kvImageGetTempBufferSize flag prevents the function from performing any processing other than to determine the minimum buffer size.

2.  After you allocate enough space for a buffer of the returned size, call the function a second time, passing a valid pointer in the `tempBuffer` parameter. This time, don’t pass the kvImageGetTempBufferSize flag.

## See Also

### Related Documentation

Adding a bokeh effect to images

Simulate a bokeh effect by applying dilation.

### Minimizing an object

func vImageMin_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes an 8-bit planar buffer.

func vImageMin_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes a 32-bit planar buffer.

func vImageMin_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes an 8-bit-per-channel, 4-channel interleaved buffer.

