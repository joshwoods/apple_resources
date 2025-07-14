

- Accelerate
-  vImagePremultipliedAlphaBlendScreen_RGBA8888(\_:\_:\_:\_:) 

Function

# vImagePremultipliedAlphaBlendScreen_RGBA8888(\_:\_:\_:\_:)

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the screen blend mode.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func vImagePremultipliedAlphaBlendScreen_RGBA8888(
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

## Mentioned in 

Compositing images with vImage blend modes

## Discussion

On return of this function, the value of each pixel in the destination buffer is:

```
// For color channels:
uint8_t destColor = CLAMP( srcTopColor + srcBottomcolor - (srcTopColor * srcBottomColor + 127)/255, 0, 255);

// For the alpha channel:
uint8_t alpha =  srcTopAlpha + ((255 - srcTopAlpha) * srcBottomAlpha + 127)/255;
```

## See Also

### Related Documentation

Compositing images with vImage blend modes

Combine two images by using blend modes to create a single output.

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Performing premultiplied alpha compositing with blend modes

func vImagePremultipliedAlphaBlendLighten_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the lighten blend mode.

func vImagePremultipliedAlphaBlendDarken_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the darken blend mode.

func vImagePremultipliedAlphaBlendMultiply_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the multiply blend mode.

