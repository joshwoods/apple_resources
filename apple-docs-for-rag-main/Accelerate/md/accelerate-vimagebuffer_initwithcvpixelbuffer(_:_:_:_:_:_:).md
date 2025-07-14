

- Accelerate
-  vImageBuffer_InitWithCVPixelBuffer(\_:\_:\_:\_:\_:\_:) 

Function

# vImageBuffer_InitWithCVPixelBuffer(\_:\_:\_:\_:\_:\_:)

Initializes a vImage buffer with a copy of the contents of a Core Video pixel buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageBuffer_InitWithCVPixelBuffer(
    _ buffer: UnsafeMutablePointer,
    _ desiredFormat: UnsafeMutablePointer,
    _ cvPixelBuffer: CVPixelBuffer,
    _ cvImageFormat: vImageCVImageFormat!,
    _ backgroundColor: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`buffer`  

The destination empty vImage_Buffer structure. On return, the function allocates new memory to the buffer and sets the buffer’s size to match the CVPixelBuffer instance’s dimensions.

`desiredFormat`  

A vImage_CGImageFormat structure that specifies the image format of the vImage_Buffer structure. If colorSpace is `nil`, the function uses sRGB.

`cvPixelBuffer`  

The source CVPixelBuffer instance. It’s not necessary to lock the pixel buffer before calling this function.

`cvImageFormat`  

An optional vImageCVImageFormat instance that specifies the pixel format of the source pixel buffer. If this parameter is `nil`, the function attempts to derive this information from the Core Video pixel buffer.

`backgroundColor`  

If the source image contains alpha information and the destination format doesn’t contain alpha information, this function flattens the source image against this parameter.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

Pass kvImageNoAllocate if the destination buffer references existing data.

If the pixel buffer uses chrominance subsampling and you want vImage to use a higher quality, but a slower, resampling filter, set the kvImageHighQualityResampling flag.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

Some Core Video pixel buffers and image formats have incompletely specified color information that prevents vImageBuffer_InitWithCVPixelBuffer(_:_:_:_:_:_:) from performing the conversion. In this situation, the function returns one of the format errors below. To proceed, create a vImageCVImageFormat instance, add the missing information, and pass the image format instance as the `cvImageFormat` parameter to this function. It’s possible that more than one piece of information is missing.

kvImageCVImageFormat_ConversionMatrix  
The conversion matrix is missing from the `cvPixelBuffer` or the `vImageCVImageFormat`. Use the vImageCVImageFormat_CopyConversionMatrix(_:_:_:) function to copy a conversion matrix to an image format.

kvImageCVImageFormat_ChromaSiting  
The chrominance siting information is missing from the `cvPixelBuffer` or the `vImageCVImageFormat`. Use vImageCVImageFormat_SetChromaSiting(_:_:) to set the chrominance siting on an image format.

kvImageCVImageFormat_ColorSpace  
The color space that contains primaries and transfer function is missing from the `cvPixelBuffer` or the `vImageCVImageFormat`. Use vImageCVImageFormat_SetColorSpace(_:_:) to set the color space on an image format.

## Discussion

For compatibility with Core Video, vImage substitutes gamma `1/1.961` for kCVImageBufferTransferFunction_ITU_R_709_2 and substitutes the ITU-R BT.709-5 transfer function for kCVImageBufferTransferFunction_SMPTE_240M_1995. You can manually set the transfer function using vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(_:_:_:_:_:) and vImageCVImageFormat_SetColorSpace(_:_:) to avoid this substitution.

