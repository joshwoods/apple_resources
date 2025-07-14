

- Accelerate
-  vImageSepConvolve_PlanarF(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageSepConvolve_PlanarF(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Convolves a floating-point 32-bit planar image by separate horizontal and vertical separable kernels.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func vImageSepConvolve_PlanarF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ srcOffsetToROI_X: vImagePixelCount,
    _ srcOffsetToROI_Y: vImagePixelCount,
    _ kernelX: UnsafePointer!,
    _ kernelX_width: UInt32,
    _ kernelY: UnsafePointer!,
    _ kernelY_width: UInt32,
    _ bias: Float,
    _ backgroundColor: Pixel_F,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

A pointer to a vImage buffer structure that contains data for the source image.

`dest`  

A pointer to a vImage buffer data structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer to which this structure points contains the destination image data. When you no longer need the data buffer, you must deallocate the memory. The size dimensions of the destination buffer also specifies the size of the region of interest in the source buffer.

`tempBuffer`  

A pointer to a temporary buffer. If you pass `NULL`, the function allocates the buffer, then deallocates it before returning. Alternatively, you can allocate the buffer yourself, in which case you’re responsible for deallocating it when you no longer need it.

`srcOffsetToROI_X`  

The horizontal offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`srcOffsetToROI_Y`  

The vertical offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`kernelX`  

A pointer to the 1D horizontal weights.

`kernelX_width`  

The number of elements in the horizontal weights array.

`kernelY`  

A pointer to the 1D vertical weights.

`kernelY_width`  

The number of elements in the vertical weights array.

`bias`  

The value to add to each element in the convolution result, before performing any clipping.

`backgroundColor`  

A background color. If you supply a color, you must also set the `kvImageBackgroundColorFill` flag, otherwise the function ignores the color.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

Pass one of the following flags to specify how vImage handles pixel locations beyond the edge of the source image: kvImageCopyInPlace, kvImageTruncateKernel, kvImageBackgroundColorFill, or kvImageEdgeExtend.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

A separable convolution applies two separate 1D filters along the rows and columns of an image in succession. This allows for a faster implementation compared to applying the corresponding 2D convolution filter.

An example of separable convolution is the edge-detection Sobel filter, for approximating the image gradient. The Sobel filter is the outer product of the averaging filter, `[1, 2, 1]`, and the differentiation filter, `[-1, 0, 1]`. For the image x-derivative, this results in the general 2D filter:

Note that the differentiation filter produces a result that contains, on average, half of the destination values having a negative value. Add a bias of 128 to allow the operation to represent values in the range `-1...1` as unsigned 8-bit integer destination pixels. For example, the operation represents a result of -1 as 0 in the destination, and represents a result of 1 as 255 in the destination.

The following code shows how to apply the averaging and differentiation components of the Sobel filter to an 8-bit planar buffer:

```
let kernelX: [Float] = [1, 2, 1]
let kernelY: [Float] = [-1, 0, 1]
let bias = Float(128)
let backgroundColor = Float(0)

// `planarSourceBuffer` contains the source image.
// `destinationBuffer` is the destination buffer, initialized by `vImageBuffer_Init`.

let error = vImageSepConvolve_PlanarF(&planarSourceBuffer,
                                      &destinationBuffer,
                                      nil,
                                      0, 0,
                                      kernelX, UInt32(kernelX.count),
                                      kernelY, UInt32(kernelY.count),
                                      bias,
                                      backgroundColor,
                                      vImage_Flags(kvImageBackgroundColorFill))
```

The following image shows two photographs, with the original image on the left, and the image after applying the Sobel filter on the right:

## See Also

### Convolving with separable filter kernels

func vImageSepConvolve_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_16U, vImage_Flags) -> vImage_Error

Convolves an 8-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_16U, vImage_Flags) -> vImage_Error

Convolves an unsigned 16-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_16F, vImage_Flags) -> vImage_Error

Convolves a floating-point 16-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_Planar8to16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Float, Pixel_8, vImage_Flags) -> vImage_Error

Convolves an 8-bit planar image by separate horizontal and vertical separable kernels, and writes the result to an unsigned 16-bit planar destination.

func vImageSepConvolve_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Convolves an 8-bit-per-channel, 4-channel interleaved image by separate horizontal and vertical separable kernels.

