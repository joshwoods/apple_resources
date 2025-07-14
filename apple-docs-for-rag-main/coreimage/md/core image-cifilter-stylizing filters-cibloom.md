

- Core Image
- CIFilter
- Stylizing Filters
-  CIBloom 

Protocol

# CIBloom

The properties you use to configure a bloom filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBloom
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

class func bloom() -> any CIFilter &amp; CIBloom

Adjusts an image’s colors by applying a blur effect.

