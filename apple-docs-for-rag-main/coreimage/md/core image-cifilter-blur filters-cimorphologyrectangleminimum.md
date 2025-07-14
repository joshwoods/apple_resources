

- Core Image
- CIFilter
- Blur Filters
-  CIMorphologyRectangleMinimum 

Protocol

# CIMorphologyRectangleMinimum

The properties you use to configure a morphology rectangle minimum filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMorphologyRectangleMinimum
```

## Topics

### Instance Properties

var height: Float

The height, in pixels, of the morphological structuring element.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var width: Float

The width, in pixels, of the morphological structuring element.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func morphologyRectangleMinimum() -> any CIFilter &amp; CIMorphologyRectangleMinimum

Blurs a rectangular area by reducing contrasting pixels.

