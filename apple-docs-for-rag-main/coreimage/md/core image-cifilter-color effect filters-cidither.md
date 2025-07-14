

- Core Image
- CIFilter
- Color Effect Filters
-  CIDither 

Protocol

# CIDither

The properties you use to configure a dither filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIDither
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var intensity: Float

The intensity of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func dither() -> any CIFilter &amp; CIDither

Applies randomized noise to produce a processed look.

