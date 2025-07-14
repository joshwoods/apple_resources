

- Accelerate
-  vImagePremultipliedAlphaBlend_BGRAFFFF(\_:\_:\_:\_:) 

Function

# vImagePremultipliedAlphaBlend_BGRAFFFF(\_:\_:\_:\_:)

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel BGRA buffers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePremultipliedAlphaBlend_BGRAFFFF(
    _ srcTop: UnsafePointer,
    _ srcBottom: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcTop`  

The vImage buffer that provides the source top image.

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
float destColor = srcTopColor  + (1.0 - srcTopAlpha) * srcBottomColor;
float alpha =  srcTopAlpha + (1.0 - srcTopAlpha) * srcBottomAlpha
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Performing premultiplied alpha compositing

func vImagePremultipliedAlphaBlend_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit planar buffers.

func vImagePremultipliedAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit planar buffers.

func vImagePremultipliedAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel ARGB buffers.

func vImagePremultipliedAlphaBlend_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel ARGB buffers.

func vImagePremultipliedAlphaBlend_BGRA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers.

