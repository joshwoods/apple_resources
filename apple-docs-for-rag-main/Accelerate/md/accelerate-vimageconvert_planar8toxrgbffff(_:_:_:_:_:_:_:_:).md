

- Accelerate
-  vImageConvert_Planar8ToXRGBFFFF(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar8ToXRGBFFFF(\_:\_:\_:\_:\_:\_:\_:\_:)

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar8ToXRGBFFFF(
    _ alpha: Pixel_F,
    _ red: UnsafePointer,
    _ green: UnsafePointer,
    _ blue: UnsafePointer,
    _ dest: UnsafePointer,
    _ maxFloat: UnsafePointer!,
    _ minFloat: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`alpha`  

The constant destination alpha value.

`red`  

The source vImage buffer that contains the red channel.

`green`  

The source vImage buffer that contains the green channel.

`blue`  

The source vImage buffer that contains the blue channel.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`maxFloat`  

The maximum pixel value for the destination image.

`minFloat`  

The minimum pixel value for the destination image.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The source and destination buffers must have the same height and width.

## See Also

### Interleaving three unsigned 8-bit planar buffers

func vImageConvert_Planar8toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an RGB565 3-channel interleaved buffer.

func vImageConvert_Planar8toRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 3-channel interleaved buffer.

func vImageConvert_Planar8ToXRGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved XRGB buffer with the specified constant alpha value.

func vImageConvert_Planar8ToBGRX8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

func vImageConvert_Planar8ToBGRXFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Interleaves three 8-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved BGRX buffer with the specified constant alpha value.

