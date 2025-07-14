

- Accelerate
-  vImageConvert_Planar8toPlanar2(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_Planar8toPlanar2(\_:\_:\_:\_:\_:)

Converts an 8-bit planar buffer to a 2-bit planar buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_Planar8toPlanar2(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ dither: Int32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `nil`, the function allocates the buffer and then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you’re responsible for deallocating it when you no longer need it.

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

### Converting from 8-bit buffers

func vImageConvert_Planar8toPlanar1(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a 1-bit planar buffer.

func vImageConvert_Planar8toPlanar4(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to a 4-bit planar buffer.

func vImageConvert_Planar8toIndexed1(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Pixel_8>, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an indexed 1-bit planar buffer.

func vImageConvert_Planar8toIndexed2(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Pixel_8>, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an indexed 2-bit planar buffer.

func vImageConvert_Planar8toIndexed4(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Pixel_8>, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an indexed 4-bit planar buffer.

func vImageConvert_Planar8To16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit planar buffer to an unsigned 16-bit planar buffer.

