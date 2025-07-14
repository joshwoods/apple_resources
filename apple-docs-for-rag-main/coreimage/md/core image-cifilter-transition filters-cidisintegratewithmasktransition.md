

- Core Image
- CIFilter
- Transition Filters
-  CIDisintegrateWithMaskTransition 

Protocol

# CIDisintegrateWithMaskTransition

The properties you use to configure a disintegrate-with-mask transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIDisintegrateWithMaskTransition
```

## Topics

### Instance Properties

var maskImage: CIImage?

An image that defines the shape to use when disintegrating from the source to the target image.

**Required**

var shadowDensity: Float

The density of the shadow the mask creates.

**Required**

var shadowOffset: CGPoint

The offset of the shadow the mask creates.

**Required**

var shadowRadius: Float

The radius of the shadow the mask creates.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func disintegrateWithMaskTransition() -> any CIFilter &amp; CIDisintegrateWithMaskTransition

Transitions between two images using a mask image.

