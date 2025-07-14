

- Core Image
- CIFilter
- Color Effect Filters
-  CIVignette 

Protocol

# CIVignette

The properties you use to configure a vignette filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIVignette
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

The distance from the center of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func vignette() -> any CIFilter &amp; CIVignette

Gradually darkens an image’s edges.

