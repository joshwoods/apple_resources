

- Accelerate
-  vImageConvert_RGB565toRGBA8888(\_:\_:\_:\_:) 

Function

# vImageConvert_RGB565toRGBA8888(\_:\_:\_:\_:)

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel RGBA buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGB565toRGBA8888(
    _ alpha: Pixel_8,
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`alpha`  

The constant destination alpha value.

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
    Pixel8 alpha = alpha
    Pixel8 red   = (5bitRedChannel   * 255 + 15) / 31
    Pixel8 green = (6bitGreenChannel * 255 + 31) / 63
    Pixel8 blue  = (5bitBlueChannel  * 255 + 15) / 31
```

## See Also

### Conversion from RGB565 16-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB565toARGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_RGB565toBGRA8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel BGRA buffer.

func vImageConvert_RGB565toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce a 4-channel ARGB1555 buffer.

func vImageConvert_RGB565toRGBA5551(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce a 4-channel RGBA5551 buffer.

