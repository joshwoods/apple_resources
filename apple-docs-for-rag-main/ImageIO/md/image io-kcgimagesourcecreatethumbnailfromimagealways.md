

- Image I/O
-  kCGImageSourceCreateThumbnailFromImageAlways 

Global Variable

# kCGImageSourceCreateThumbnailFromImageAlways

A Boolean value that indicates whether to always create a thumbnail image.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageSourceCreateThumbnailFromImageAlways: CFString
```

## Discussion

The value of this key is a CFBoolean. The default value is kCFBooleanFalse.

If you set the value of this key to kCFBooleanTrue, the image source creates the thumbnail from the full image, subject to the limit specified by kCGImageSourceThumbnailMaxPixelSize. If you don’t specify a maximum pixel size, the image source creates the thumbnail using the image’s full size, which in most cases is not desirable.

Include this key in the options dictionary you pass to the function CGImageSourceCreateThumbnailAtIndex(_:_:_:).

## See Also

### Specifying the Read Options

let kCGImageSourceTypeIdentifierHint: CFString

The uniform type identifier that represents your best guess for the image’s type.

let kCGImageSourceShouldAllowFloat: CFString

A Boolean that indicates whether to use floating-point values in returned images.

let kCGImageSourceShouldCache: CFString

A Boolean value that indicates whether to cache the decoded image.

let kCGImageSourceShouldCacheImmediately: CFString

A Boolean value that indicates whether image decoding and caching happens at image creation time.

let kCGImageSourceCreateThumbnailFromImageIfAbsent: CFString

A Boolean value that indicates whether to create a thumbnail image automatically if the data source doesn’t contain one.

let kCGImageSourceThumbnailMaxPixelSize: CFString

The maximum width and height of a thumbnail image, specified in pixels.

let kCGImageSourceCreateThumbnailWithTransform: CFString

A Boolean value that indicates whether to rotate and scale the thumbnail image to match the image’s orientation and aspect ratio.

let kCGImageSourceSubsampleFactor: CFString

The factor by which to scale down any returned images.

