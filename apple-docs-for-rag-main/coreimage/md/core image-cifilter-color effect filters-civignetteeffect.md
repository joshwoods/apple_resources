

- Core Image
- CIFilter
- Color Effect Filters
-  CIVignetteEffect 

Protocol

# CIVignetteEffect

The properties you use to configure a vignette-effect filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIVignetteEffect
```

## Topics

### Instance Properties

var center: CGPoint

The center of the effect as x and y coordinates.

**Required**

var falloff: Float

The falloff of the effect.

**Required**

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

class func vignetteEffect() -> any CIFilter &amp; CIVignetteEffect

Gradually darkens a specified area of an image.

