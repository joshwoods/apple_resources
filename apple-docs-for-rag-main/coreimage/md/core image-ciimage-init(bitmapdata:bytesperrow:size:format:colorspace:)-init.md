

- Core Image
- CIImage
-  init(bitmapData:bytesPerRow:size:format:colorSpace:) 

Initializer

# init(bitmapData:bytesPerRow:size:format:colorSpace:)

Initializes an image object with bitmap data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(
    bitmapData data: Data,
    bytesPerRow: Int,
    size: CGSize,
    format: CIFormat,
    colorSpace: CGColorSpace?
)
```

## Parameters 

`d`  

The bitmap data to use for the image. The data you supply must be premultiplied.

`bpr`  

The number of bytes per row.

`size`  

The size of the image data.

`f`  

A pixel format constant. See `Pixel Formats`.

`c`  

The color space that the image is defined in. It must be a Quartz 2D color space (CGColorSpace). Pass `nil` for images that don’t contain color data (such as elevation maps, normal vector maps, and sampled function tables).

## Return Value

The initialized image object.

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

init(cvImageBuffer: CVImageBuffer, options: [CIImageOption : Any]?)

Initializes an image object from the contents of a Core Video image buffer, using the specified options.

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

+ imageWithBitmapData:bytesPerRow:size:format:colorSpace:

Creates and returns an image object from bitmap data.

