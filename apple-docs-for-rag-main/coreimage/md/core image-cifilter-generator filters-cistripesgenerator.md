

- Core Image
- CIFilter
- Generator Filters
-  CIStripesGenerator 

Protocol

# CIStripesGenerator

The properties you use to configure a stripes generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIStripesGenerator
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the stripe pattern.

**Required**

var color0: CIColor

A color to use for the odd stripes.

**Required**

var color1: CIColor

A color to use for the even stripes.

**Required**

var sharpness: Float

The sharpness of the stripe pattern.

**Required**

var width: Float

The width of a stripe.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func stripesGenerator() -> any CIFilter &amp; CIStripesGenerator

Generates a line of stripes as an image

