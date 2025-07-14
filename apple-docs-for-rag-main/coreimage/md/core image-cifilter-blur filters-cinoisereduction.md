

- Core Image
- CIFilter
- Blur Filters
-  CINoiseReduction 

Protocol

# CINoiseReduction

The properties you use to configure a noise reduction filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CINoiseReduction
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var noiseLevel: Float

The amount of noise reduction.

**Required**

var sharpness: Float

The sharpness of the final image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func noiseReduction() -> any CIFilter &amp; CINoiseReduction

Reduces noise by sharpening the edges of objects.

