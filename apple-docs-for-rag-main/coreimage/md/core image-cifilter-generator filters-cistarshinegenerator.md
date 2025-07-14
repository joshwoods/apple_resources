

- Core Image
- CIFilter
- Generator Filters
-  CIStarShineGenerator 

Protocol

# CIStarShineGenerator

The properties you use to configure a star-shine generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIStarShineGenerator
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the star.

**Required**

var color: CIColor

The color to use for the outer shell of the circular star.

**Required**

var crossAngle: Float

The angle of the cross pattern.

**Required**

var crossOpacity: Float

The opacity of the cross pattern.

**Required**

var crossScale: Float

The size of the cross pattern.

**Required**

var crossWidth: Float

The width of the cross pattern.

**Required**

var epsilon: Float

The length of the cross spikes.

**Required**

var radius: Float

The radius of the star.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func starShineGenerator() -> any CIFilter &amp; CIStarShineGenerator

Generates a star-shine image.

