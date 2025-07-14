

- Accelerate
- vImage_Buffer
-  init(cgImage:format:flags:) 

Initializer

# init(cgImage:format:flags:)

Creates a new buffer with the contents of a Core Graphics image using the supplied image format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    cgImage: CGImage,
    format: vImage_CGImageFormat,
    flags options: vImage.Options = .noFlags
) throws
```

## Parameters 

`cgImage`  

The source image.

`format`  

The desired image format.

`options`  

The options to use when performing the operation.

## Mentioned in 

Creating and Populating Buffers from Core Graphics Images

## Discussion

This function converts the source Core Graphics image that the `cgImage` parameter specifies to the format that the `format` parameter describes.

For example, the following code converts a color image to grayscale and initializes the vImage buffer with the planar monochrome image data:

```
let format = vImage_CGImageFormat(
    bitsPerComponent: 8,
    bitsPerPixel: 8,
    colorSpace: CGColorSpaceCreateDeviceGray(),
    bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.none.rawValue))!

// `cgImage` is a color image.
let buffer = try vImage_Buffer(cgImage: cgImage,
                               format: format)
```

## See Also

### Consuming and producing Core Graphics images

init(cgImage: CGImage, flags: vImage.Options) throws

Creates a new buffer with the contents of a Core Graphics image.

func createCGImage(format: vImage_CGImageFormat, flags: vImage.Options) throws -> CGImage

Creates a Core Graphics image from the vImage buffer.

