

- Accelerate
-  vImageConvert_Planar16Q12toARGB8888(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar16Q12toARGB8888(\_:\_:\_:\_:\_:\_:)

Interleaves four fixed-point 16-bit planar buffers into an 8-bit-per-channel, 4-channel interleaved buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar16Q12toARGB8888(
    _ alpha: UnsafePointer,
    _ red: UnsafePointer,
    _ green: UnsafePointer,
    _ blue: UnsafePointer,
    _ dest: UnsafePointer,
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

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
uint8_t dest = clamp(src, 0, 4096)*255 + 2048 >> 12
```

The conversion maps source pixels with a value of `0` to `0` and source pixels with a value of `4088` or greater to `255`.

## See Also

### Interleaving four fixed-point 16-bit planar buffers

func vImageConvert_Planar16Q12toARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Interleaves four fixed-point 16-bit planar buffers into a floating-point 32-bit-per-channel, 4-channel interleaved buffer.

