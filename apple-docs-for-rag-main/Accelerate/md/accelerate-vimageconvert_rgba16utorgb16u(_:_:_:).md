

- Accelerate
-  vImageConvert_RGBA16UtoRGB16U(\_:\_:\_:) 

Function

# vImageConvert_RGBA16UtoRGB16U(\_:\_:\_:)

Removes the alpha channel from an unsigned 16-bit-per-channel RGBA buffer to produce an unsigned 16-bit-per-channel RGB result.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGBA16UtoRGB16U(
    _ rgbaSrc: UnsafePointer,
    _ rgbDest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`rgbaSrc`  

The source vImage buffer.

`rgbDest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

This function copies the red, green, and blue source channels to the destination buffer.

## See Also

### Conversion from unsigned 16-bit-per-channel, 4-channel interleaved buffers

func vImageConvert_ARGB16UtoRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an unsigned 16-bit-per-channel ARGB buffer to produce an unsigned 16-bit-per-channel RGB result.

func vImageConvert_BGRA16UtoRGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Removes the alpha channel from an unsigned 16-bit-per-channel BGRA buffer to produce an unsigned 16-bit-per-channel RGB result.

