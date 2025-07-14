

- Accelerate
-  vImageVerticalReflect_CbCr16F(\_:\_:\_:) 

Function

# vImageVerticalReflect_CbCr16F(\_:\_:\_:)

Reflects a floating-point 16-bit-per-channel, 2-channel interleaved image vertically across the center horizontal line.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func vImageVerticalReflect_CbCr16F(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to a vImage buffer structure that contains the source image.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile, otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function doesn’t scale or resample; instead, it copies unchanged individual pixels to new locations. The source and destination buffers must have the same height and the same width.

This function doesn’t work in place — that is, the source and destination buffers must point to different memory.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Applying vertical reflection to 16-bit-per-channel buffers

func vImageVerticalReflect_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an unsigned 16-bit planar image vertically across the center horizontal line.

func vImageVerticalReflect_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit planar image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an unsigned 16-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a signed 16-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

