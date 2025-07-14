

- Accelerate
-  vImageConvert_BGRA8888toRGB888(\_:\_:\_:) 

Function

# vImageConvert_BGRA8888toRGB888(\_:\_:\_:)

Removes the alpha channel from an 8-bit-per-channel BGRA buffer to produce an 8-bit-per-channel RGB result.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 6.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_BGRA8888toRGB888(
    _: UnsafePointer,
    _: UnsafePointer,
    _: vImage_Flags
) -> vImage_Error
```

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function copies the red, green, and blue source channels to the destination buffer.

### Parameters

bgraSrc  
The source vImage buffer.

rgbDest  
A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

flags  
The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## See Also

### Conversion from 8-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_RGBA8888toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel RGBA buffer to produce an 8-bit-per-channel RGB result.

func vImageConvert_ARGB8888toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an 8-bit-per-channel ARGB buffer to produce an RGB565 result.

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

