

- Accelerate
-  vImageAlphaBlend_Planar8(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageAlphaBlend_Planar8(\_:\_:\_:\_:\_:\_:\_:)

Performs nonpremultiplied alpha compositing of two 8-bit planar buffers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageAlphaBlend_Planar8(
    _ srcTop: UnsafePointer,
    _ srcTopAlpha: UnsafePointer,
    _ srcBottom: UnsafePointer,
    _ srcBottomAlpha: UnsafePointer,
    _ alpha: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcTop`  

The vImage buffer that provides the source top image.

`srcTopAlpha`  

The vImage buffer that provides the source top alpha.

`srcBottom`  

The vImage buffer that provides the source bottom image.

`srcBottomAlpha`  

The vImage buffer that provides the source bottom alpha.

`alpha`  

The source vImage buffer that provides the precalculated alpha values of the composite image. Precalculate these values by calling the function vImagePremultipliedAlphaBlend_Planar8(_:_:_:_:_:).

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

In order to provide the best performance, this function doesn’t calculate the alpha channel for the composite image. Use the following code to calculate the alpha channel for the composite image that you pass to this function as the `alpha` parameter:

```
vImagePremultipliedAlphaBlend_Planar8(srcTopAlpha,
                                      srcTopAlpha,
                                      srcBottomAlpha,
                                      alpha,
                                      vImage_Flags(kvImageNoFlags))
```

On return of vImagePremultipliedAlphaBlend_Planar8(_:_:_:_:_:), the value of each pixel in the alpha buffer is:

```
float alpha = srcTopAlpha + (1.0 - srcTopAlpha) * srcBottomAlpha
```

If you’re performing an alpha blend on multiple-channel data, such as an RGB image, use the same alpha channel buffer for each call to this function.

On return of this function, the value of each pixel in the destination buffer is:

```
float destColor = (  srcTopColor * srcTopAlpha + (1.0 - srcTopAlpha) * srcBottomAlpha * srcBottomColor ) / alpha
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Performing nonpremultiplied alpha compositing

func vImageAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit planar buffers.

func vImageAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit-per-channel, 4-channel ARGB buffers.

func vImageAlphaBlend_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 32-bit-per-channel, 4-channel ARGB buffers.

