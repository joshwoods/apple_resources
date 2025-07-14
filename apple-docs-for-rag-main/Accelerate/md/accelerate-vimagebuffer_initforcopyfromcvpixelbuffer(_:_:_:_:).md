

- Accelerate
-  vImageBuffer_InitForCopyFromCVPixelBuffer(\_:\_:\_:\_:) 

Function

# vImageBuffer_InitForCopyFromCVPixelBuffer(\_:\_:\_:\_:)

Initializes an array of vImage buffers in the order necessary to copy from a Core Video pixel buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageBuffer_InitForCopyFromCVPixelBuffer(
    _ buffers: UnsafeMutablePointer,
    _ converter: vImageConverter,
    _ pixelBuffer: CVPixelBuffer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`buffers`  

An array of vImage_Buffer structures. The number of source buffers is the return value of vImageConverter_GetNumberOfSourceBuffers(_:).

`converter`  

A Core-Video-to-Core-Graphics vImageConverter instance.

`pixelBuffer`  

A locked CVPixelBuffer instance.

`flags`  

The options to use when performing this operation.

Important

Always pass the kvImageNoAllocate flag to this function. The kvImageNoAllocate flag instructs the function to initialize the buffers to read directly from a locked CVPixelBuffer instance. All operations that use the buffers must be between calls to the CVPixelBufferLockBaseAddress(_:_:) and CVPixelBufferUnlockBaseAddress(_:_:) functions.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The vImage library represents multiple plane Core Video pixel buffers as individual vImage buffers. Call vImageConverter_GetNumberOfSourceBuffers(_:) to instantiate the correct number of source buffers. Use this function to initialize the vImage buffers that you pass as the sources to a Core-Video-to-Core-Graphics vImageConverter instance.

The following shows the code for creating the three source buffers required to represent a kCVPixelFormatType_420YpCbCr8Planar pixel buffer. On return of vImageBuffer_InitForCopyFromCVPixelBuffer(_:_:_:_:), the three vImage buffers contain the luminance, Cb, and Cr image data.

```
let colorSpace = CGColorSpaceCreateDeviceRGB()

guard
    let cvImageFormat = vImageCVImageFormat.make(
        format: .format420YpCbCr8Planar,
        matrix: kvImage_ARGBToYpCbCrMatrix_ITU_R_709_2.pointee,
        chromaSiting: .center,
        colorSpace: colorSpace,
        alphaIsOpaqueHint: false),

    var cgImageFormat = vImage_CGImageFormat(
        bitsPerComponent: 8,
        bitsPerPixel: 32,
        colorSpace: colorSpace,
        bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.noneSkipFirst.rawValue),
        renderingIntent: .defaultIntent),

    let converterCVtoCG = try? vImageConverter.make(
        sourceFormat: cvImageFormat,
        destinationFormat: cgImageFormat) else {
    return
}

let sourceBufferCount = vImageConverter_GetNumberOfSourceBuffers(converterCVtoCG)
var sourceBuffers = (0 ..

## See Also

### Initializing vImage buffers that reference Core Video pixel buffer data

func vImageBuffer_InitForCopyToCVPixelBuffer(UnsafeMutablePointer&lt;vImage_Buffer>, vImageConverter, CVPixelBuffer, vImage_Flags) -> vImage_Error

Initializes an array of vImage buffers in the order necessary to copy to a Core Video pixel buffer.

