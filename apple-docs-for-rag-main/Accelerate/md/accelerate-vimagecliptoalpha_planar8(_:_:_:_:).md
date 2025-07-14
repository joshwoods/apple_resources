

- Accelerate
-  vImageClipToAlpha_Planar8(\_:\_:\_:\_:) 

Function

# vImageClipToAlpha_Planar8(\_:\_:\_:\_:)

Clamps the values of an 8-bit planar buffer to the corresponding alpha values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageClipToAlpha_Planar8(
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

On return of this function, the value of each pixel in the destination buffer is:

```
color_result = MIN( color, alpha )
```

## See Also

### Clipping color values to alpha

func vImageClipToAlpha_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of a 32-bit planar buffer to the corresponding alpha values.

func vImageClipToAlpha_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of an 8-bit-per-channel, 4-channel ARGB buffer to the corresponding alpha values.

func vImageClipToAlpha_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of an 8-bit-per-channel, 4-channel RGBA buffer to the corresponding alpha values.

func vImageClipToAlpha_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of a 32-bit-per-channel, 4-channel ARGB buffer to the corresponding alpha values.

func vImageClipToAlpha_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of a 32-bit-per-channel, 4-channel RGBA buffer to the corresponding alpha values.

