

- Accelerate
-  vImagePremultiplyData_PlanarF(\_:\_:\_:\_:) 

Function

# vImagePremultiplyData_PlanarF(\_:\_:\_:\_:)

Transforms a 32-bit planar buffer from nonpremultiplied alpha format to premultiplied alpha format.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePremultiplyData_PlanarF(
    _ src: UnsafePointer,
    _ alpha: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`alpha`  

The vImage buffer that provides the source alpha.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function multiplies color channels by the alpha channel using the following code:

```
uint8_t destColor = (src * alpha + 127) / 255;
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Converting from unpremultiplied to premultiplied format

func vImagePremultiplyData_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit planar buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 32-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 32-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

