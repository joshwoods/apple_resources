

- Accelerate
-  vImageConvert_RGB565toRGBA5551(\_:\_:\_:\_:) 

Function

# vImageConvert_RGB565toRGBA5551(\_:\_:\_:\_:)

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce a 4-channel RGBA5551 buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGB565toRGBA5551(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ dither: Int32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`dither`  

The dithering algorithm.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function supports the following dithering algorithms:

kvImageConvert_DitherNone  
Doesn’t apply any dithering. This algorithm rounds the input values to the nearest representable value in the destination format.

kvImageConvert_DitherOrdered  
Adds precomputed blue noise to the source image before it rounds the input values to the nearest representable value in the destination format. The vImage conversion functions support uniform and Gaussian noise by including kvImageConvert_OrderedUniformBlue and kvImageConvert_OrderedGaussianBlue, respectively.

kvImageConvert_DitherOrderedReproducible  
Returns the same result as kvImageConvert_DitherOrdered but uses the same offset into the blue noise for each call.

kvImageConvert_DitherFloydSteinberg  
Applies Floyd-Steinberg dithering to the image.

kvImageConvert_DitherAtkinson  
Applies Atkinson dithering to the image.

## See Also

### Related Documentation

Improving the quality of quantized images with dithering

Apply dithering to simulate colors that are unavailable in reduced bit depths.

### Conversion from RGB565 16-bit-per-channel, 3-channel interleaved buffers

func vImageConvert_RGB565toARGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel ARGB buffer.

func vImageConvert_RGB565toBGRA8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel BGRA buffer.

func vImageConvert_RGB565toRGBA8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce an 8-bit-per-channel, 4-channel RGBA buffer.

func vImageConvert_RGB565toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int32, vImage_Flags) -> vImage_Error

Combines an RGB565 3-channel RGB buffer and a constant alpha value to produce a 4-channel ARGB1555 buffer.

