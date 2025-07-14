

- Accelerate
-  vImageConvert_RGBA5551toRGB565(\_:\_:\_:) 

Function

# vImageConvert_RGBA5551toRGB565(\_:\_:\_:)

Removes the alpha channel from an RGBA5551 buffer to produce an RGB565 result.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGBA5551toRGB565(
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

This function copies the red, green, and blue source channels to the destination buffer.

## See Also

### Conversion from ARGB1555 16-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB1555toRGB565(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an ARGB1555 buffer to produce an RGB565 result.

