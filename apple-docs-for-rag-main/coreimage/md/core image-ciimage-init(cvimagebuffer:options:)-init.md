

- Core Image
- CIImage
-  init(cvImageBuffer:options:) 

Initializer

# init(cvImageBuffer:options:)

Initializes an image object from the contents of a Core Video image buffer, using the specified options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(
    cvImageBuffer imageBuffer: CVImageBuffer,
    options: [CIImageOption : Any]? = nil
)
```

## Parameters 

`imageBuffer`  

A `CVImageBuffer` object in a supported pixel format constant. For more information, see Core Video Programming Guide and Core Video.

`dict`  

A dictionary that contains options for creating an image object. (See `Image Dictionary Keys`.) The pixel format is supplied by the `CVImageBuffer` object.)

## Return Value

The initialized image object.

## Discussion

The `imageBuffer` parameter must be in one of the following formats:

- kCVPixelFormatType_32ARGB

- kCVPixelFormatType_422YpCbCr8

- kCVPixelFormatType_32BGRA

## See Also

### Creating an Image

class func empty() -> CIImage

Creates and returns an empty image object.

init?(image: UIImage)

Initializes an image object with the specified UIKit image object.

init?(image: UIImage, options: [CIImageOption : Any]?)

Initializes an image object with the specified UIKit image object, using the specified options.

init?(contentsOf: URL)

Initializes an image object by reading an image from a URL.

init?(contentsOf: URL, options: [CIImageOption : Any]?)

Initializes an image object by reading an image from a URL, using the specified options.

init(cgImage: CGImage)

Initializes an image object with a Quartz 2D image.

init(cgImage: CGImage, options: [CIImageOption : Any]?)

Initializes an image object with a Quartz 2D image, using the specified options.

init(cgImageSource: CGImageSource, index: Int, options: [CIImageOption : Any]?)

init?(data: Data)

Initializes an image object with the supplied image data.

init?(data: Data, options: [CIImageOption : Any]?)

Initializes an image object with the supplied image data, using the specified options.

init(bitmapData: Data, bytesPerRow: Int, size: CGSize, format: CIFormat, colorSpace: CGColorSpace?)

Initializes an image object with bitmap data.

init?(bitmapImageRep: NSBitmapImageRep)

Initializes an image object with the specified bitmap image representation.

init(imageProvider: Any, size: Int, Int, format: CIFormat, colorSpace: CGColorSpace?, options: [CIImageOption : Any]?)

Initializes an image object with data provided by an image provider, using the specified options.

init?(depthData: AVDepthData)

init?(depthData: AVDepthData, options: [String : Any]?)

init?(portaitEffectsMatte: AVPortraitEffectsMatte)

init?(portaitEffectsMatte: AVPortraitEffectsMatte, options: [CIImageOption : Any]?)

init?(semanticSegmentationMatte: AVSemanticSegmentationMatte)

init?(semanticSegmentationMatte: AVSemanticSegmentationMatte, options: [CIImageOption : Any]?)

init(cvImageBuffer: CVImageBuffer)

Initializes an image object from the contents of a Core Video image buffer.

init(cvPixelBuffer: CVPixelBuffer)

Initializes an image object from the contents of a Core Video pixel buffer.

init(cvPixelBuffer: CVPixelBuffer, options: [CIImageOption : Any]?)

Initializes an image object from the contents of a Core Video pixel buffer using the specified options.

init?(mtlTexture: any MTLTexture, options: [CIImageOption : Any]?)

Initializes an image object with data supplied by a Metal texture.

init(ioSurface: IOSurfaceRef)

Initializes an image with the contents of an IOSurface.

init(ioSurface: IOSurfaceRef, options: [CIImageOption : Any]?)

Initializes, using the specified options, an image with the contents of an IOSurface.

### Related Documentation

+ imageWithCVImageBuffer:options:

Creates and returns an image object from the contents of `CVImageBuffer` object, using the specified options.

