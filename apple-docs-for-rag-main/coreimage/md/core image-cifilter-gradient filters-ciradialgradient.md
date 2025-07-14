

- Core Image
- CIFilter
- Gradient Filters
-  CIRadialGradient 

Protocol

# CIRadialGradient

The properties you use to configure a radial gradient filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIRadialGradient
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

var radius0: Float

The radius of the starting circle to use in the gradient.

**Required**

var radius1: Float

The radius of the ending circle to use in the gradient.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func radialGradient() -> any CIFilter &amp; CIRadialGradient

Generates a gradient that varies radially between two circles having the same center.

