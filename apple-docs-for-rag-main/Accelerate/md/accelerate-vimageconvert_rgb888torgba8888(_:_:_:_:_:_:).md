

- Accelerate
-  vImageConvert_RGB888toRGBA8888(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_RGB888toRGBA8888(\_:\_:\_:\_:\_:\_:)

Combines an 8-bit-per-channel, 3-channel RGB buffer and either an 8-bit alpha buffer or constant alpha value to produce an RGBA result.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 6.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGB888toRGBA8888(
    _: UnsafePointer,
    _: UnsafePointer!,
    _: Pixel_8,
    _: UnsafePointer,
    _: Bool,
    _: vImage_Flags
) -> vImage_Error
```

## Discussion

### Parameters

rgbSrc  
The source vImage buffer that contains the red, green, and blue channels.

aSrc  
The source vImage buffer that contains the alpha channel. Set this value to `nil` to specify that the function sets the destination alpha as the constant destination alpha value.

alpha  
The constant destination alpha value. The function ignores this paramater if the `aSrc` parameter isn’t `nil`.

rgbaDest  
A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

premultiply  
A Boolean value that specifes whether the function premultiplies the color channels by the alpha channel.

flags  
The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

Returns  
kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

If you specify `premultiply` as `true`, the function uses the following calculation to perform the conversion:

```
 r = (a * r + 127) / 255
 g = (a * g + 127) / 255
 b = (a * b + 127) / 255
```

## See Also

### Conversion from 8-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB888toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an 8-bit-per-channel, 3-channel RGB buffer and either an 8-bit alpha buffer or constant alpha value to produce an ARGB result.

func vImageConvert_RGB888toBGRA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_8, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an 8-bit-per-channel, 3-channel RGB buffer and either an 8-bit alpha buffer or constant alpha value to produce a BGRA result.

