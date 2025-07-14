

- Accelerate
-  vImageConvert_Planar8toRGB565(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar8toRGB565(\_:\_:\_:\_:\_:)

Interleaves three 8-bit planar buffers into an RGB565 3-channel interleaved buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar8toRGB565(
    _ srcR: UnsafePointer,
    _ srcG: UnsafePointer,
    _ srcB: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

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
    uint32_t red   = (8bitRedChannel   * (31*2) + 255) / (255*2)
    uint32_t green = (8bitGreenChannel * 63 + 127) / 255
    uint32_t blue  = (8bitBlueChannel  * 31 + 127) / 255
    uint16_t RGB565pixel = (red 

## See Also

### Interleaving three unsigned 8-bit planar buffers

func vImageConvert_Planar8toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 3-channel interleaved buffer.

func vImageConvert_Planar8ToXRGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

func vImageConvert_Planar8ToBGRX8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

func vImageConvert_Planar8ToXRGBFFFF(Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

func vImageConvert_Planar8ToBGRXFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

