

- Core Image
- CIImage
-  init(imageProvider:size:\_:format:colorSpace:options:) 

Initializer

# init(imageProvider:size:\_:format:colorSpace:options:)

Initializes an image object with data provided by an image provider, using the specified options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(
    imageProvider p: Any,
    size width: Int,
    _ height: Int,
    format f: CIFormat,
    colorSpace cs: CGColorSpace?,
    options: [CIImageOption : Any]? = nil
)
```

## Parameters 

`p`  

A data provider that implements the CIImageProvider informal protocol. Core Image maintains a strong reference to this object until the image is deallocated.

`width`  

The width of the image data.

`height`  

The height of the image data.

`f`  

A pixel format constant. See `Pixel Formats`.

`cs`  

The color space of the image. If this value is `nil`, the image is not color matched. Pass `nil` for images that don’t contain color data (such as elevation maps, normal vector maps, and sampled function tables).

`dict`  

A dictionary that specifies image-creation options, either `kCIImageProviderTileSize` or `kCIImageProviderUserInfo`. See `CIImageProvider` for more information on these options.

## Return Value

The initialized image object.

## Discussion

Core Image does not populate the image until it needs the data.

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

+ imageWithImageProvider:size::format:colorSpace:options:

Creates and returns an image object initialized with data provided by an image provider.

