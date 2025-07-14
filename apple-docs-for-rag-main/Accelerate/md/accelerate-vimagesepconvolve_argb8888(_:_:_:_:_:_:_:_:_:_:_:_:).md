

- Accelerate
-  vImageSepConvolve_ARGB8888(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageSepConvolve_ARGB8888(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Convolves an 8-bit-per-channel, 4-channel interleaved image by separate horizontal and vertical separable kernels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func vImageSepConvolve_ARGB8888(
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
    _ backgroundColor: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`tempBuffer`  

A pointer to an optional buffer that the function uses as a workspace during the convolution operation. Pass `nil` to specify that the function allocates and deallocates its own temporary buffer. Pass the kvImageGetTempBufferSize flag to specify that the function returns the required temporary buffer size for a set of parameters.

`srcOffsetToROI_X`  

The horizontal offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`srcOffsetToROI_Y`  

The vertical offset, in pixels, to the upper-left pixel of the region of interest within the source image.

`kernelX`  

A pointer to the 32-bit floating-point horizontal convolution weights.

`kernelX_width`  

The number of elements in the horizontal convolution kernel.

`kernelY`  

A pointer to the 32-bit floating-point vertical convolution weights.

`kernelY_width`  

The number of elements in the vertical convolution kernel.

`bias`  

The value that the operation adds to each element in the convolution result.

`backgroundColor`  

The background color that the function applies when you pass the kvImageBackgroundColorFill flag.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

Pass one of the following flags to specify how vImage handles pixel locations beyond the edge of the source image: kvImageCopyInPlace, kvImageTruncateKernel, kvImageBackgroundColorFill, or kvImageEdgeExtend.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## See Also

### Convolving with separable filter kernels

func vImageSepConvolve_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_16U, vImage_Flags) -> vImage_Error

Convolves an 8-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_16U, vImage_Flags) -> vImage_Error

Convolves an unsigned 16-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_16F, vImage_Flags) -> vImage_Error

Convolves a floating-point 16-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Pixel_F, vImage_Flags) -> vImage_Error

Convolves a floating-point 32-bit planar image by separate horizontal and vertical separable kernels.

func vImageSepConvolve_Planar8to16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>!, UInt32, UnsafePointer&lt;Float>!, UInt32, Float, Float, Pixel_8, vImage_Flags) -> vImage_Error

Convolves an 8-bit planar image by separate horizontal and vertical separable kernels, and writes the result to an unsigned 16-bit planar destination.

