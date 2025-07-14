

- Image I/O
-  kCGImageSourceTypeIdentifierHint 

Global Variable

# kCGImageSourceTypeIdentifierHint

The uniform type identifier that represents your best guess for the image’s type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageSourceTypeIdentifierHint: CFString
```

## Discussion

The value of this key is a CFString object. Add this key to the options dictionary when you create a CGImageSource object.

## See Also

### Specifying the Read Options

let kCGImageSourceShouldAllowFloat: CFString

A Boolean that indicates whether to use floating-point values in returned images.

let kCGImageSourceShouldCache: CFString

A Boolean value that indicates whether to cache the decoded image.

let kCGImageSourceShouldCacheImmediately: CFString

A Boolean value that indicates whether image decoding and caching happens at image creation time.

let kCGImageSourceCreateThumbnailFromImageIfAbsent: CFString

A Boolean value that indicates whether to create a thumbnail image automatically if the data source doesn’t contain one.

let kCGImageSourceCreateThumbnailFromImageAlways: CFString

A Boolean value that indicates whether to always create a thumbnail image.

let kCGImageSourceThumbnailMaxPixelSize: CFString

The maximum width and height of a thumbnail image, specified in pixels.

let kCGImageSourceCreateThumbnailWithTransform: CFString

A Boolean value that indicates whether to rotate and scale the thumbnail image to match the image’s orientation and aspect ratio.

let kCGImageSourceSubsampleFactor: CFString

The factor by which to scale down any returned images.

