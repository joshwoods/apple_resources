

- Accelerate
-  vImageFloodFill_ARGB8888(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageFloodFill_ARGB8888(\_:\_:\_:\_:\_:\_:\_:)

Applies a flood-fill operation to an 8-bit-per-channel, four-channel interleaved image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func vImageFloodFill_ARGB8888(
    _ srcDest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ seedX: vImagePixelCount,
    _ seedY: vImagePixelCount,
    _ newValue: UnsafeMutablePointer!,
    _ connectivity: Int32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcDest`  

A pointer to a vImage buffer structure that contains the source image and receives the destination image. This function always works in place, that is, the input and the output point to the same memory.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `nil`, the function allocates the buffer and then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you’re responsible for deallocating it when you no longer need it.

`seedX`  

The x-coordinate that defines the position of the seed pixel inside the connected component.

`seedY`  

The y-coordinate that defines the position of the seed pixel inside the connected component.

`newValue`  

The new pixel value that overwrites the pixels in the connected component.

`connectivity`  

An integer that specifies which pixels the operation includes as neighbors. Pass either `4` or `8`. The four-connected neighborhood of a pixel are the pixels to the left and right, and those above and below. The eight-connected neighborhood also includes the pixels on the four diagonals.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Mentioned in 

Applying flood fills to an image

## Discussion

The flood-fill function sets all pixels that are neighboring and identical to the seed pixel to a new color. The operation continues until it reaches the image boundary or until it sets all pixels within the connected component to the new value.

## See Also

### Flood-filling buffers

Applying flood fills to an image

Fill consistently colored connected parts of an image with a new color.

func vImageFloodFill_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, Pixel_8, Int32, vImage_Flags) -> vImage_Error

Applies a flood-fill operation to an 8-bit planar image.

func vImageFloodFill_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, Pixel_16U, Int32, vImage_Flags) -> vImage_Error

Applies a flood fill-operation to an unsigned 16-bit planar image.

func vImageFloodFill_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafeMutablePointer&lt;UInt16>!, Int32, vImage_Flags) -> vImage_Error

Applies a flood-fill operation to an unsigned 16-bit-per-channel, four-channel interleaved image.

