

- AppKit
- NSAdaptiveImageGlyph
-  contentIdentifier 

Instance Property

# contentIdentifier

A unique identifier for this image.

macOS 15.0+

``` source
var contentIdentifier: String { get }
```

## Discussion

Use this property to create a persistent reference to this specific image in your code. The image data contains this content identifier, so the value persists between instantiations.

## See Also

### Getting the content metadata

var contentDescription: String

An alternate textual description of the image contents.

class var contentType: UTType

The image data format to use for this image type.

