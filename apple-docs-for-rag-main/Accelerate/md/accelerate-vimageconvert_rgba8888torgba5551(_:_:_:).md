

- Accelerate
-  vImageConvert_RGBA8888toRGBA5551(\_:\_:\_:) 

Function

# vImageConvert_RGBA8888toRGBA5551(\_:\_:\_:)

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGBA8888toRGBA5551(
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

The RGBA5551 format has 16-bit pixels with 1 bit for alpha and 5 bits each for red, green, and blue. The function uses the following calculation to perform the conversion:

```
 uint32_t red   = (8bitRedChannel   * 31 + 127) / 255;
 uint32_t green = (8bitGreenChannel * 31 + 127) / 255;
 uint32_t blue  = (8bitBlueChannel  * 31 + 127) / 255;
 uint32_t alpha = (8bitAlphaChannel      + 127) / 255;
 dest->data[x] =  (red 

## See Also

### Converting from 8-bit buffers

func vImageConvert_RGB888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 3-channel interleaved buffer to an RGB565 3-channel interleaved buffer using the specified dithering algorithm.

func vImageConvert_ARGB8888toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer.

func vImageConvert_ARGB8888toARGB1555_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer usng the specified dithering algorithm.

func vImageConvert_RGBA8888toRGBA5551_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer usng the specified dithering algorithm.

func vImageConvert_ARGB8888ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel buffer with permutation.

