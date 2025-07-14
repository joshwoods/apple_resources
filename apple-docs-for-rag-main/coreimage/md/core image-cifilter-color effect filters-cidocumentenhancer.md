

- Core Image
- CIFilter
- Color Effect Filters
-  CIDocumentEnhancer 

Protocol

# CIDocumentEnhancer

The properties you use to configure a document enhancer filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIDocumentEnhancer
```

## Topics

### Instance Properties

var amount: Float

The amount of enhancement.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func documentEnhancer() -> any CIFilter &amp; CIDocumentEnhancer

Adjusts an image’s shadows and contrast.

