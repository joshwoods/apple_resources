

- Core Image
- CIFilter
- Generator Filters
-  CIAttributedTextImageGenerator 

Protocol

# CIAttributedTextImageGenerator

The properties you use to configure an attributed-text image generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIAttributedTextImageGenerator
```

## Topics

### Instance Properties

var scaleFactor: Float

The scale at which to render the text.

**Required**

var text: NSAttributedString

The text to render.

**Required**

var padding: Float

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func attributedTextImageGenerator() -> any CIFilter &amp; CIAttributedTextImageGenerator

Generates an attributed-text image.

