

- Core Image
- CIFilter
- Gradient Filters
-  CIHueSaturationValueGradient 

Protocol

# CIHueSaturationValueGradient

The properties you use to configure a hue-saturation-value gradient filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIHueSaturationValueGradient
```

## Topics

### Instance Properties

var colorSpace: CGColorSpace?

The color space for the generated color wheel.

**Required**

var dither: Float

A Boolean value specifying whether the dither the generated output.

**Required**

var radius: Float

The distance from the center of the effect.

**Required**

var softness: Float

The softness of the generated color wheel.

**Required**

var value: Float

The lightness of the hue-saturation gradient.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func hueSaturationValueGradient() -> any CIFilter &amp; CIHueSaturationValueGradient

Generates a gradient representing a specified color space.

