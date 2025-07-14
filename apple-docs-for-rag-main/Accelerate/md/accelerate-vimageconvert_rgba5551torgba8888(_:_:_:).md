

- Accelerate
-  vImageConvert_RGBA5551toRGBA8888(\_:\_:\_:) 

Function

# vImageConvert_RGBA5551toRGBA8888(\_:\_:\_:)

Converts an RGB5651 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGBA5551toRGBA8888(
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
    Pixel8 alpha =  1bitAlphaChannel * 255
    Pixel8 red   = (5bitRedChannel   * 255 + 15) / 31
    Pixel8 green = (5bitGreenChannel * 255 + 15) / 31
    Pixel8 blue  = (5bitBlueChannel  * 255 + 15) / 31
```

## See Also

### Converting from ARGB1555 16-bit-per-channel buffers

func vImageConvert_ARGB1555toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an ARGB1555 4-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer.

