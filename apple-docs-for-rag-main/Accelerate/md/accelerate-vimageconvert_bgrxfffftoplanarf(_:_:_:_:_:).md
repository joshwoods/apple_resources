

- Accelerate
-  vImageConvert_BGRXFFFFToPlanarF(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_BGRXFFFFToPlanarF(\_:\_:\_:\_:\_:)

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into three floating-point 32-bit planar buffers and discards the last channel.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_BGRXFFFFToPlanarF(
    _ src: UnsafePointer,
    _ blue: UnsafePointer,
    _ green: UnsafePointer,
    _ red: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`blue`  

A pointer to the blue destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the blue destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`green`  

A pointer to the green destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the green destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`red`  

A pointer to the red destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the red destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The source and destination buffers must have the same height and width.

## See Also

### Deinterleaving 32-bit four-channel interleaved buffers

func vImageConvert_ARGBFFFFtoPlanar8(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into four 8-bit planar buffers.

func vImageConvert_XRGBFFFFToPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into three floating-point 32-bit planar buffers and discards the first channel.

func vImageConvert_ARGBFFFFtoPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Deinterleaves a floating-point 32-bit-per-channel, 4-channel interleaved buffer into four floating-point 38-bit planar buffers.

