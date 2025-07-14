

- Accelerate
-  vImagePremultiplyData_RGBA16U(\_:\_:\_:) 

Function

# vImagePremultiplyData_RGBA16U(\_:\_:\_:)

Transforms an unsigned 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 6.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePremultiplyData_RGBA16U(
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

This function multiplies color channels by the alpha channel using the following code:

```
uint16_t destColor = (src * alpha + 32767) / 65535;
uint16_t destAlpha = alpha;
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Converting from unpremultiplied to premultiplied format

func vImagePremultiplyData_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit planar buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit planar buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

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

