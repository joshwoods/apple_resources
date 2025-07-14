

- AppKit
- NSAdaptiveImageGlyph
-  contentDescription 

Instance Property

# contentDescription

An alternate textual description of the image contents.

macOS 15.0+

``` source
var contentDescription: String { get }
```

## Discussion

This string contains a brief description of the image, which is useful for searches or places where you need a text-based description. The adaptive image derives the content of this property from the underlying image data.

## See Also

### Getting the content metadata

var contentIdentifier: String

A unique identifier for this image.

class var contentType: UTType

The image data format to use for this image type.

