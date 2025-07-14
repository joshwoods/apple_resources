

- Core Image
- CIFilter
- Gradient Filters
-  CILinearGradient 

Protocol

# CILinearGradient

The properties you use to configure a linear gradient filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CILinearGradient
```

## Topics

### Instance Properties

var color0: CIColor

The first color to use in the gradient.

**Required**

var color1: CIColor

The second color to use in the gradient.

**Required**

var point0: CGPoint

The starting position of the gradient.

**Required**

var point1: CGPoint

The ending position of the gradient.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func linearGradient() -> any CIFilter &amp; CILinearGradient

Generates a color gradient that varies along a linear axis between two defined endpoints.

