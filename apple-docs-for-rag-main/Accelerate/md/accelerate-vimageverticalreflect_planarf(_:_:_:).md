

- Accelerate
-  vImageVerticalReflect_PlanarF(\_:\_:\_:) 

Function

# vImageVerticalReflect_PlanarF(\_:\_:\_:)

Reflects a 32-bit planar image vertically across the center horizontal line.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageVerticalReflect_PlanarF(
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

### Applying vertical reflection to 32-bit-per-channel buffers

func vImageVerticalReflect_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a 32-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

