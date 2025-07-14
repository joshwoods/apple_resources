

- Core Image
- CIFilter
- Generator Filters
-  CITextImageGenerator 

Protocol

# CITextImageGenerator

The properties you use to configure a text image generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CITextImageGenerator
```

## Topics

### Instance Properties

var fontName: String

The name of the font to use for the generated text.

**Required**

var fontSize: Float

The size of the font to use for the generated text.

**Required**

var scaleFactor: Float

The scale of the font to use for the generated text.

**Required**

var text: String

The text to render.

**Required**

var padding: Float

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func textImageGenerator() -> any CIFilter &amp; CITextImageGenerator

Generates a text image.

