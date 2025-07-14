

- Image I/O
-  kCGImageSourceShouldCache 

Global Variable

# kCGImageSourceShouldCache

A Boolean value that indicates whether to cache the decoded image.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageSourceShouldCache: CFString
```

## Discussion

The value of this key is a CFBoolean. The default value is kCFBooleanTrue for 64-bit architectures, and kCFBooleanFalse for 32-bit architectures.

Include this key in the options dictionary you pass to the functions CGImageSourceCopyPropertiesAtIndex(_:_:_:) and CGImageSourceCreateImageAtIndex(_:_:_:).

## See Also

### Specifying the Read Options

let kCGImageSourceTypeIdentifierHint: CFString

The uniform type identifier that represents your best guess for the image’s type.

let kCGImageSourceShouldAllowFloat: CFString

A Boolean that indicates whether to use floating-point values in returned images.

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

