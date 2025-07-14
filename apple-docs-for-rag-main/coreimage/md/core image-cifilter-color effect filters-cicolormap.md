

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorMap 

Protocol

# CIColorMap

The properties you use to configure a color map filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorMap
```

## Topics

### Instance Properties

var gradientImage: CIImage?

The image data that transforms the source image values.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorMap() -> any CIFilter &amp; CIColorMap

Performs a transformation of the input image colors to colors from a gradient image.

