

- Accelerate
-  vImageConvert_RGB16UToARGB8888(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_RGB16UToARGB8888(\_:\_:\_:\_:\_:\_:)

Converts an unsigned 16-bit-per-channel, 3-channel interleaved buffer to an 8-bit-per-channel, 4-channel interleaved buffer using permutation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGB16UToARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ permuteMap: UnsafePointer,
    _ copyMask: UInt8,
    _ backgroundColor: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`copyMask`  

A bitmask that specifies the channel from the background color that the function copies to the destination channel at the corresponding index. The `1000` bit corresponds to the alpha channel, the `0100` bit corresponds to the red channel, the `0010` corresponds to the green channel, and the `0001` bit corresponds to the blue channel.

`backgroundColor`  

A 16-bit-per-channel, 4-channel pixel value that replaces the destination pixels based on the copy mask.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function doesn’t work in place.

## See Also

### Conversion from unsigned 16-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB16UtoARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_16U, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an unsigned 16-bit-per-channel, 3-channel RGB buffer and either an unsigned 16-bit alpha buffer or constant alpha value to produce an ARGB result.

func vImageConvert_RGB16UtoBGRA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_16U, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an unsigned 16-bit-per-channel, 3-channel RGB buffer and either an unsigned 16-bit alpha buffer or constant alpha value to produce a BGRA result.

func vImageConvert_RGB16UtoRGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>!, Pixel_16U, UnsafePointer&lt;vImage_Buffer>, Bool, vImage_Flags) -> vImage_Error

Combines an unsigned 16-bit-per-channel, 3-channel RGB buffer and either an unsigned 16-bit alpha buffer or constant alpha value to produce an RGBA result.

