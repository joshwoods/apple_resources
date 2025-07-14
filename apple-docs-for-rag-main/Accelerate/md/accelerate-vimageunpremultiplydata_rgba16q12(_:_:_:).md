

- Accelerate
-  vImageUnpremultiplyData_RGBA16Q12(\_:\_:\_:) 

Function

# vImageUnpremultiplyData_RGBA16Q12(\_:\_:\_:)

Transforms a fixed-point 16-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageUnpremultiplyData_RGBA16Q12(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function divides color channels by the alpha channel using the following code:

```
int16_t destColor = ( MIN(src_color, alpha) * 4096 + alpha/2) / alpha;
int16_t destAlpha = alpha;
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Converting from premultiplied to unpremultiplied format

func vImageUnpremultiplyData_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit planar buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit planar buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 16-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

