

- Accelerate
-  vImageConvert_Fto16Q12(\_:\_:\_:) 

Function

# vImageConvert_Fto16Q12(\_:\_:\_:)

Converts a floating-point 32-bit planar buffer to a fixed-point 16-bit planar buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Fto16Q12(
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

The conversion maps source pixels with a value of `0.0` to `0` and `1.0` to `4096`.

## See Also

### Converting from floating-point 32-bit-per-channel buffers

func vImageConvert_PlanarFtoPlanar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to a floating-point 16-bit planar buffer.

