

- Core Image
- CIFilter
- Generator Filters
-  CISunbeamsGenerator 

Protocol

# CISunbeamsGenerator

The properties you use to configure a sunbeams generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISunbeamsGenerator
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the sunbeam pattern.

**Required**

var color: CIColor

The color of the sun.

**Required**

var maxStriationRadius: Float

The radius of the sunbeams.

**Required**

var striationContrast: Float

The contrast of the sunbeams.

**Required**

var striationStrength: Float

The intensity of the sunbeams.

**Required**

var sunRadius: Float

The radius of the sun.

**Required**

var time: Float

The duration of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func sunbeamsGenerator() -> any CIFilter &amp; CISunbeamsGenerator

Generates an image resembling the sun.

