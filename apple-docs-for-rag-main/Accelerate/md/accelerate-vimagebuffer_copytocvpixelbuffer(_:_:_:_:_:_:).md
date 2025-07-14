

- Accelerate
-  vImageBuffer_CopyToCVPixelBuffer(\_:\_:\_:\_:\_:\_:) 

Function

# vImageBuffer_CopyToCVPixelBuffer(\_:\_:\_:\_:\_:\_:)

Copies the contents of a vImage buffer to a Core Video pixel buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageBuffer_CopyToCVPixelBuffer(
    _ buffer: UnsafePointer,
    _ bufferFormat: UnsafePointer,
    _ cvPixelBuffer: CVPixelBuffer,
    _ cvImageFormat: vImageCVImageFormat!,
    _ backgroundColor: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`buffer`  

The source vImage buffer.

`bufferFormat`  

A vImage_CGImageFormat structure that specifies the image format of the vImage_Buffer structure. If colorSpace is `nil`, the function uses sRGB.

`cvPixelBuffer`  

The destination CVPixelBuffer instance. It’s not necessary to lock the pixel buffer before calling this function.

`cvImageFormat`  

An optional vImageCVImageFormat instance that specifies the pixel format of the source pixel buffer. If this parameter is `nil`, the function attempts to derive this information from the Core Video pixel buffer.

`backgroundColor`  

If the source image contains alpha information and the destination format doesn’t contain alpha information, this function flattens the source image against this parameter.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

For compatibility with Core Video, vImage substitutes gamma `1/1.961` for kCVImageBufferTransferFunction_ITU_R_709_2 and substitutes the ITU-R BT.709-5 transfer function for kCVImageBufferTransferFunction_SMPTE_240M_1995. You can manually set the transfer function using vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(_:_:_:_:_:) and vImageCVImageFormat_SetColorSpace(_:_:) to avoid this substitution.

