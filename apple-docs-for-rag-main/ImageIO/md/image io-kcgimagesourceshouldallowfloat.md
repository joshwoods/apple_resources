

- Image I/O
-  kCGImageSourceShouldAllowFloat 

Global Variable

# kCGImageSourceShouldAllowFloat

A Boolean that indicates whether to use floating-point values in returned images.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageSourceShouldAllowFloat: CFString
```

## Discussion

The value of this key is a CFBoolean. The default value is kCFBooleanFalse, which tells the image source not to use floating-point values.

If the image format supports floating-point values, this key tells the image source to format CGImage types using those values. The use of extended-range floating-point values may require additional processing to render in a pleasing manner.

## See Also

### Specifying the Read Options

let kCGImageSourceTypeIdentifierHint: CFString

The uniform type identifier that represents your best guess for the image’s type.

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

