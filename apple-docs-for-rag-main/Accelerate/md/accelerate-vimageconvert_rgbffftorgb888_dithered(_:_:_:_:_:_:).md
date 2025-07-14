

- Accelerate
-  vImageConvert_RGBFFFtoRGB888_dithered(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConvert_RGBFFFtoRGB888_dithered(\_:\_:\_:\_:\_:\_:)

Converts a floating-point 32-bit-per-channel, 3-channel buffer to an 8-bit-per-channel, 3-channel buffer using the specified dithering algorithm.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGBFFFtoRGB888_dithered(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ maxFloat: UnsafePointer,
    _ minFloat: UnsafePointer,
    _ dither: Int32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`maxFloat`  

The three maximum source pixel values.

`minFloat`  

The three minumum source pixel values.

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

### Converting from floating-point 32-bit-per-channel buffers

func vImageConvert_ARGBFFFFtoARGB8888_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, Int32, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit-per-channel, 4-channel buffer to an 8-bit-per-channel, 4-channel buffer using the specified dithering algorithm.

