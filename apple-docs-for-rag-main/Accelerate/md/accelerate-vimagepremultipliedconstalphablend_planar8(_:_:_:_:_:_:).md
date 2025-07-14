

- Accelerate
-  vImagePremultipliedConstAlphaBlend_Planar8(\_:\_:\_:\_:\_:\_:) 

Function

# vImagePremultipliedConstAlphaBlend_Planar8(\_:\_:\_:\_:\_:\_:)

Performs premultiplied alpha compositing of two 8-bit planar buffers and applies an extra alpha value to the top buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePremultipliedConstAlphaBlend_Planar8(
    _ srcTop: UnsafePointer,
    _ constAlpha: Pixel_8,
    _ srcTopAlpha: UnsafePointer,
    _ srcBottom: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcTop`  

The vImage buffer that provides the source top image.

`constAlpha`  

The constant alpha value that the function applies to the top image.

`srcTopAlpha`  

The vImage buffer that provides the source top alpha.

`srcBottom`  

The vImage buffer that provides the source bottom image.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

On return of this function, the value of each pixel in the destination buffer is:

```
uint8_t destColor = (srcTopColor * constAlpha * 255  + (255*255 - srcTopAlpha * constAlpha) * srcBottomColor + 127*255) / (255*255);
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Performing premultiplied alpha compositing with a single alpha value

func vImagePremultipliedConstAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit planar buffers and applies an extra alpha value to the top buffer.

func vImagePremultipliedConstAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel interleaved buffers and applies an extra alpha value to the top buffer.

func vImagePremultipliedConstAlphaBlend_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel interleaved buffers and applies an extra alpha value to the top buffer.

