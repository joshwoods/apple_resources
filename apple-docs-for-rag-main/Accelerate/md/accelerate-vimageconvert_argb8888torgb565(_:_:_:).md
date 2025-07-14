

- Accelerate
-  vImageConvert_ARGB8888toRGB565(\_:\_:\_:) 

Function

# vImageConvert_ARGB8888toRGB565(\_:\_:\_:)

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an RGB565 result.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_ARGB8888toRGB565(
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

The function uses the following calculation to perform the conversion:

```
    uint32_t red   = (8bitRedChannel   * (31*2) + 255) / (255*2)
    uint32_t green = (8bitGreenChannel * 63 + 127) / 255
    uint32_t blue  = (8bitBlueChannel  * 31 + 127) / 255
    uint16_t RGB565pixel = (red 

## See Also

### Conversion from 8-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_RGBA8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_BGRA8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel BGRA buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_ARGB8888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer using the specified dithering algorithm to produce an RGB565 result.

func vImageConvert_BGRA8888toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an RGB565 result.

func vImageConvert_BGRA8888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel BGRA buffer using the specified dithering algorithm to produce an RGB565 result.

func vImageConvert_RGBA8888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer using the specified dithering algorithm to produce an RGB565 result.

func vImageConvert_RGBA8888toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an RGB565 result.

func vImageConvert_ARGB8888ToRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an unsigned 16-bit-per-channel RGB result.

