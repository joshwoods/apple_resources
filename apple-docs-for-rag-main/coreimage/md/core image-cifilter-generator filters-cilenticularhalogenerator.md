

- Core Image
- CIFilter
- Generator Filters
-  CILenticularHaloGenerator 

Protocol

# CILenticularHaloGenerator

The properties you use to configure a lenticular halo generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CILenticularHaloGenerator
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the halo.

**Required**

var color: CIColor

The color of the halo.

**Required**

var haloOverlap: Float

The separation of colors in the halo.

**Required**

var haloRadius: Float

The radius of the halo.

**Required**

var haloWidth: Float

The width of the halo, from its inner radius to its outer radius.

**Required**

var striationContrast: Float

The contrast of the halo colors.

**Required**

var striationStrength: Float

The intensity of the halo colors.

**Required**

var time: Float

The current time of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func lenticularHaloGenerator() -> any CIFilter &amp; CILenticularHaloGenerator

Generates a lenticular halo image.

