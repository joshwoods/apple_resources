

- Accelerate
-  vImageConvert_RGB888toPlanar8(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_RGB888toPlanar8(\_:\_:\_:\_:\_:)

Deinterleaves an 8-bit-per-channel, 3-channel interleaved buffer into three 8-bit planar buffers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGB888toPlanar8(
    _ rgbSrc: UnsafePointer,
    _ redDest: UnsafePointer,
    _ greenDest: UnsafePointer,
    _ blueDest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`rgbSrc`  

The source vImage buffer.

`redDest`  

A pointer to the red destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the red destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`greenDest`  

A pointer to the green destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the green destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`blueDest`  

A pointer to the blue destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the blue destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The source and destination buffers must have the same height and width.

## See Also

### Deinterleaving unsigned 8-bit, three-channel interleaved buffers

func vImageConvert_RGB888toPlanar16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves an 8-bit-per-channel, 3-channel interleaved buffer into three fixed-point 16-bit planar buffers.

