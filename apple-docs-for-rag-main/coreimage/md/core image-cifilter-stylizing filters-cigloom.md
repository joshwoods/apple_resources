

- Core Image
- CIFilter
- Stylizing Filters
-  CIGloom 

Protocol

# CIGloom

The properties you use to configure a gloom filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIGloom
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var intensity: Float

The intensity of the effect.

**Required**

var radius: Float

The radius, in pixels, of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func gloom() -> any CIFilter &amp; CIGloom

Adjusts an image’s color by applying a gloom filter.

