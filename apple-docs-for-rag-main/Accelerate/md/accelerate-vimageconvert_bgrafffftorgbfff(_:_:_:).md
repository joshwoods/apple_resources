

- Accelerate
-  vImageConvert_BGRAFFFFtoRGBFFF(\_:\_:\_:) 

Function

# vImageConvert_BGRAFFFFtoRGBFFF(\_:\_:\_:)

Removes the alpha channel from a floating-point 32-bit-per-channel BGRA buffer to produce a floating-point 32-bit-per-channel RGB result.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_BGRAFFFFtoRGBFFF(
    _ src: UnsafePointer!,
    _ dest: UnsafePointer!,
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

This function copies the red, green, and blue source channels to the destination buffer.

## See Also

### Conversion from 32-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGBFFFFtoRGBFFF(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Removes the alpha channel from a floating-point 32-bit-per-channel ARGB buffer to produce a floating-point 32-bit-per-channel RGB result.

func vImageConvert_RGBAFFFFtoRGBFFF(UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Removes the alpha channel from a floating-point 32-bit-per-channel RGBA buffer to produce a floating-point 32-bit-per-channel RGB result.

