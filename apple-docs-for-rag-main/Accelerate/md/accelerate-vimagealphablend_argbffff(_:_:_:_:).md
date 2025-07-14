

- Accelerate
-  vImageAlphaBlend_ARGBFFFF(\_:\_:\_:\_:) 

Function

# vImageAlphaBlend_ARGBFFFF(\_:\_:\_:\_:)

Performs nonpremultiplied alpha compositing of two 32-bit-per-channel, 4-channel ARGB buffers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageAlphaBlend_ARGBFFFF(
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

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

## Return Value

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Discussion

On return of this function, the value of each pixel in the destination buffer is:

```
float alpha =  srcTopAlpha + (1.0 - srcTopAlpha) * srcBottomAlpha
float destColor = (  srcTopColor * srcTopAlpha + (1.0 - srcTopAlpha) * srcBottomAlpha * srcBottomColor ) / alpha
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Performing nonpremultiplied alpha compositing

func vImageAlphaBlend_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit planar buffers.

func vImageAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit planar buffers.

func vImageAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit-per-channel, 4-channel ARGB buffers.

