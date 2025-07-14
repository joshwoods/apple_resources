

- Core Image
- CIFilter
- Gradient Filters
-  CIGaussianGradient 

Protocol

# CIGaussianGradient

The properties you use to configure a Gaussian gradient filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIGaussianGradient
```

## Topics

### Instance Properties

var center: CGPoint

The center of the effect as x and y coordinates.

**Required**

var color0: CIColor

The first color to use in the gradient.

**Required**

var color1: CIColor

The second color to use in the gradient.

**Required**

var radius: Float

The radius of the Gaussian distribution.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func gaussianGradient() -> any CIFilter &amp; CIGaussianGradient

Generates a gradient that varies from one color to another using a Gaussian distribution.

