

- Core Image
- CIFilter
- Color Effect Filters
-  CIFalseColor 

Protocol

# CIFalseColor

The properties you use to configure a false color filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIFalseColor
```

## Topics

### Instance Properties

var color0: CIColor

The first color to use for the color ramp.

**Required**

var color1: CIColor

The second color to use for the color ramp.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func falseColor() -> any CIFilter &amp; CIFalseColor

Replaces an image’s colors with specified colors.

