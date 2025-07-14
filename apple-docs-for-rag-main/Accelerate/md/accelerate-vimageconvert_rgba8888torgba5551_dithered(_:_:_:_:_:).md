

- Accelerate
-  vImageConvert_RGBA8888toRGBA5551_dithered(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_RGBA8888toRGBA5551_dithered(\_:\_:\_:\_:\_:)

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer usng the specified dithering algorithm.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_RGBA8888toRGBA5551_dithered(
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

kvImageConvert_DitherOrdered  
Adds precomputed blue noise to the source image before it rounds the input values to the nearest representable value in the destination format. The vImage conversion functions support uniform and Gaussian noise by including kvImageConvert_OrderedUniformBlue and kvImageConvert_OrderedGaussianBlue, respectively.

kvImageConvert_DitherOrderedReproducible  
Returns the same result as kvImageConvert_DitherOrdered but uses the same offset into the blue noise for each call.

## See Also

### Related Documentation

Improving the quality of quantized images with dithering

Apply dithering to simulate colors that are unavailable in reduced bit depths.

### Converting from 8-bit buffers

func vImageConvert_RGB888toRGB565_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 3-channel interleaved buffer to an RGB565 3-channel interleaved buffer using the specified dithering algorithm.

func vImageConvert_ARGB8888toARGB1555(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer.

func vImageConvert_ARGB8888toARGB1555_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Int32, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an ARGB1555 4-channel interleaved buffer usng the specified dithering algorithm.

func vImageConvert_RGBA8888toRGBA5551(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an RGBA5551 4-channel interleaved buffer.

func vImageConvert_ARGB8888ToARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Converts an 8-bit-per-channel, 4-channel interleaved buffer to an unsigned 16-bit-per-channel, 4-channel buffer with permutation.

