

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIHueAdjust 

Protocol

# CIHueAdjust

The properties you use to configure a hue adjust filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIHueAdjust
```

## Topics

### Instance Properties

var angle: Float

An angle, in radians, to use to correct the hue of an image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func hueAdjust() -> any CIFilter &amp; CIHueAdjust

Modifies an image’s hue.

