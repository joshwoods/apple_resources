

- Accelerate
-  vImageConvert_Planar1toPlanar8(\_:\_:\_:) 

Function

# vImageConvert_Planar1toPlanar8(\_:\_:\_:)

Converts a 1-bit planar buffer to an 8-bit planar buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar1toPlanar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

Because the source pixel format is smaller than a byte, there are multiple pixels in each byte of the data buffer. This function interprets pixels as big-endian order. That is, the low-indexed pixel is in the high-order bits of the byte. For example, the eight 1-bit pixels `0b11100011` map to the eight 8-bit pixels `[255, 255, 255, 0, 0, 0, 255, 255]`.

The conversion ignores any unused bits of the final byte of a row when a scanline ends in the middle of a byte.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The conversion uses the source pixel value multiplied by `255` as the corresponding destination pixel value.

## See Also

### Converting from 1-bit buffers

func vImageConvert_Indexed1toPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Converts an indexed 1-bit planar buffer to an 8-bit planar buffer.

