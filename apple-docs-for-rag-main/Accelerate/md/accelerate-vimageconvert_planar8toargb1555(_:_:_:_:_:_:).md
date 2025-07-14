

- Accelerate
-  vImageConvert_Planar8toARGB1555(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar8toARGB1555(\_:\_:\_:\_:\_:\_:)

Interleaves four 8-bit planar buffers into an ARGB1555 4-channel interleaved buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar8toARGB1555(
    _ srcA: UnsafePointer,
    _ srcR: UnsafePointer,
    _ srcG: UnsafePointer,
    _ srcB: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcA`  

The source vImage buffer that contains the alpha channel.

`srcR`  

The source vImage buffer that contains the red channel.

`srcG`  

The source vImage buffer that contains the green channel.

`srcB`  

The source vImage buffer that contains the blue channel.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
    Pixel8 alpha =  1bitAlphaChannel * 255
    Pixel8 red   = (5bitRedChannel   * 255 + 15) / 31
    Pixel8 green = (5bitGreenChannel * 255 + 15) / 31
    Pixel8 blue  = (5bitBlueChannel  * 255 + 15) / 31
```

## See Also

### Interleaving four unsigned 8-bit planar buffers

func vImageConvert_Planar8toARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageConvert_Planar8ToARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves four 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved ARGB buffer.

