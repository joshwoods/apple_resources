

- Core Image
- CIFilter
- Transition Filters
-  CIRippleTransition 

Protocol

# CIRippleTransition

The properties you use to configure a ripple transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIRippleTransition
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var extent: CGRect

A rectangle that defines the extent of the effect.

**Required**

var scale: Float

A value that determines whether the ripple starts as a bulge (a higher value) or a dimple (a lower value).

**Required**

var shadingImage: CIImage?

An image that looks like a shaded sphere enclosed in a square.

**Required**

var width: Float

The width of the ripple.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func rippleTransition() -> any CIFilter &amp; CIRippleTransition

Simulates a ripple in a pond to transiton from one image to another.

