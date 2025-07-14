

- AppKit
- NSAdaptiveImageGlyph
-  contentType 

Type Property

# contentType

The image data format to use for this image type.

macOS 15.0+

``` source
class var contentType: UTType { get }
```

## Discussion

Use this type when you need to specify the type of the image data. Adaptive images are compatible with the HEIC format, but include extra metadata about the supported resolutions and sizes.

## See Also

### Getting the content metadata

var contentIdentifier: String

A unique identifier for this image.

var contentDescription: String

An alternate textual description of the image contents.

