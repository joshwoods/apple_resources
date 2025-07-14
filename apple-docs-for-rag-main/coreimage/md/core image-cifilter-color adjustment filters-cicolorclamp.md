

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIColorClamp 

Protocol

# CIColorClamp

The properties you use to configure a color clamp filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorClamp
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var maxComponents: CIVector

A vector containing the higher clamping values.

**Required**

var minComponents: CIVector

A vector containing the lower clamping values.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorClamp() -> any CIFilter &amp; CIColorClamp

Alters the colors in an image based on color components.

