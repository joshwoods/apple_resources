

- Accelerate
-  vImageConvert_PlanarFToARGB8888(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_PlanarFToARGB8888(\_:\_:\_:\_:\_:\_:\_:\_:)

Interleaves four 32-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_PlanarFToARGB8888(
    _ alpha: UnsafePointer,
    _ red: UnsafePointer,
    _ green: UnsafePointer,
    _ blue: UnsafePointer,
    _ dest: UnsafePointer,
    _ maxFloat: UnsafePointer,
    _ minFloat: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`alpha`  

The source vImage buffer that contains the alpha channel.

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

The function uses the following calculation to perform the conversion:

```
uint8_t result = SATURATED_CLIP_0_to_255( 255.0f * ( srcPixel - minFloat ) / (maxFloat - minFloat) + 0.5f );
```

## See Also

### Interleaving four floating-point 32-bit planar buffers

func vImageConvert_PlanarFtoARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four floating-point 32-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel ARGB interleaved buffer.

func vImageConvert_PlanarFToBGRXFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four floating-point 32-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel BGRXARGB interleaved buffer.

