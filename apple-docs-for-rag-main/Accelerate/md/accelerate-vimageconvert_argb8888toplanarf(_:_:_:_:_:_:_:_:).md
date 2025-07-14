

- Accelerate
-  vImageConvert_ARGB8888toPlanarF(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_ARGB8888toPlanarF(\_:\_:\_:\_:\_:\_:\_:\_:)

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into four floating-point 32-bit planar buffers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_ARGB8888toPlanarF(
    _ src: UnsafePointer!,
    _ alpha: UnsafePointer!,
    _ red: UnsafePointer!,
    _ green: UnsafePointer!,
    _ blue: UnsafePointer!,
    _ maxFloat: UnsafePointer!,
    _ minFloat: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`alpha`  

A pointer to the alpha destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the alpha destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`red`  

A pointer to the red destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the red destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`green`  

A pointer to the green destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the green destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`blue`  

A pointer to the blue destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the blue destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

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
 float result = (maxFloat - minFloat) * (float) srcPixel / 255.0  + minFloat
```

The source and destination buffers must have the same height and width.

## See Also

### Deinterleaving unsigned 8-bit, four-channel interleaved buffers

func vImageConvert_BGRX8888ToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into three 8-bit planar buffers and discards the last channel.

func vImageConvert_XRGB8888ToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into three 8-bit planar buffers and discards the first channel.

func vImageConvert_ARGB8888toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into four 8-bit planar buffers.

func vImageConvert_ARGB8888toPlanar16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 4-channel interleaved buffer into four fixed-point 16-bit planar buffers.

