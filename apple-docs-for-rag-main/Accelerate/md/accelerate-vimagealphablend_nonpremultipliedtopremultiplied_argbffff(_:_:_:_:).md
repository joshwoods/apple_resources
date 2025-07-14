

- Accelerate
-  vImageAlphaBlend_NonpremultipliedToPremultiplied_ARGBFFFF(\_:\_:\_:\_:) 

Function

# vImageAlphaBlend_NonpremultipliedToPremultiplied_ARGBFFFF(\_:\_:\_:\_:)

Composites a nonpremultiplied 32-bit-per-channel, ARGB buffer over a premultiplied ARGB buffer and generates a premultiplied result.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageAlphaBlend_NonpremultipliedToPremultiplied_ARGBFFFF(
    _ srcTop: UnsafePointer,
    _ srcBottom: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcTop`  

The vImage buffer that provides the nonpremultiplied source top image.

`srcBottom`  

The vImage buffer that provides the premultiplied source bottom image.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

On return of this function, the value of each pixel in the destination buffer is:

```
result = srcTop * srcTopAlpha + (1 - srcTopAlpha) * srcBottom;
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Performing nonpremultiplied to premultiplied alpha compositing

func vImageAlphaBlend_NonpremultipliedToPremultiplied_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 8-bit planar buffer over a premultiplied 8-bit planar buffer and generates a premultiplied result.

func vImageAlphaBlend_NonpremultipliedToPremultiplied_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 32-bit planar buffer over a premultiplied 32-bit planar buffer and generates a premultiplied result.

func vImageAlphaBlend_NonpremultipliedToPremultiplied_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 8-bit-per-channel, ARGB buffer over a premultiplied ARGB buffer and generates a premultiplied result.

